<script>
export default {
  components: {},
  data: () => {
    return {
      PublicItems: [
        {
          id: 1,
          title: "publicpool.Guardian",
          content: "publicpool.Content2",
          titleColor: "#16ff90",
        },
        {
          id: 2,
          title: "publicpool.Bundler",
          content: "publicpool.Content3",
          titleColor: "#8aa8f3",
        },
        {
          id: 3,
          title: "publicpool.CryptoThought",
          content: "publicpool.Content6",
          titleColor: "#8aa8f3",
        },
        {
          id: 4,
          title: "publicpool.EipsFun",
          content: "publicpool.Content4",
          titleColor: "#8aa8f3",
        },
        {
          id: 5,
          title: "publicpool.ETHHackathonTeamService",
          content: "publicpool.Content8",
          titleColor: "#c8aff6",
        },
        {
          id: 6,
          title: "publicpool.Seas",
          content: "publicpool.Content9",
          titleColor: "#00ff85",
        },
        {
          id: 7,
          title: "publicpool.EthDeSocialNetwork",
          content: "publicpool.Content7",
          titleColor: "#c8aff6",
        },
        {
          id: 8,
          title: "publicpool.Scaffold",
          content: "publicpool.Content5",
          titleColor: "#00ff85",
        },
      ],
    };
  },
  computed: {},
  methods: {
    setbgcolor(_color) {
      return { backgroundColor: _color };
    },
  },
  mounted() {},
};
</script>

<template>
  <!-- Projects grid -->

  <section id="PublicPool" class="pt-10 pb-5 text-left sm:pt-14">
    <div class="flex mb-10 max-[782px]:flex-col max-[782px]:px-5">
      <h1 class="min-[781px]:pl-5 text-3xl font-extrabold">
        {{ $t("publicpool.Publicpool") }}
      </h1>
      <span
        class="flex items-center justify-center min-[781px]:pl-6 max-[781px]:mt-3"
      >
        {{ $t("publicpool.Content1") }}
      </span>
    </div>
    <div class="grid grid-cols-2 gap-4 px-5 min-[781px]:grid-cols-3">
      <div
        class="bg-white border border-gray-500 rounded-lg shadow-lg"
        v-for="item in PublicItems"
        :key="item.id"
      >
        <div
          class="flex justify-between p-5 text-3xl font-semibold text-left rounded-t-lg"
          :style="setbgcolor(item.titleColor)"
        >
          <h6 class="max-[500px]:text-sm">{{ $t(item.title) }}</h6>
          <i data-feather="chevron-right" class="group-hover:text-green-400">
          </i>
        </div>
        <div class="py-10 px-5 text-left max-[500px]:text-sm">
          {{ $t(item.content) }}
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
