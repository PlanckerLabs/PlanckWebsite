<script>
export default {
  components: {},
  data: () => {
    return {
      PreResearchItems: [
        {
          id: 1,
          title: "preresearch.Recursive",
          content: "preresearch.Content2",
          titleColor: "#16ff90",
          href: "https://recursive.plancker.org/",
        },
        {
          id: 2,
          title: "preresearch.Xhash",
          content: "preresearch.Content3",
          titleColor: "#8aa8f3",
          href: "https://xhash.com/",
        },
        {
          id: 3,
          title: "preresearch.RemixChina",
          content: "preresearch.Content4",
          titleColor: "#8aa8f3",
          href: "https://github.com/PlanckerLabs/remix-china",
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
  <section id="Research" class="pt-2 pb-20 sm:pt-14">
    <div class="flex mb-10">
      <h1 class="pl-5 text-3xl font-extrabold">
        {{ $t("preresearch.PreResearchGroup") }}
      </h1>
      <span class="flex items-center justify-center pl-6">
        {{ $t("preresearch.Content1") }}
      </span>
    </div>
    <div class="grid grid-cols-1 gap-4 px-5 min-[781px]:grid-cols-3">
      <a
        class="flex items-stretch"
        v-for="item in this.PreResearchItems"
        :key="item.id"
        :href="item.href"
        target="_blank"
      >
        <div
          class="items-stretch w-full bg-white border border-gray-500 rounded-lg shadow-lg prbg"
        >
          <div
            class="flex justify-between p-5 text-3xl font-semibold text-left border-b border-gray-300 rounded-t-lg"
          >
            <h6 class="max-[500px]:text-sm">{{ $t(item.title) }}</h6>
            <i data-feather="chevron-right" class="group-hover:text-green-400">
            </i>
          </div>
          <div class="py-10 px-5 text-left max-[500px]:text-sm">
            {{ $t(item.content) }}
          </div>
        </div>
      </a>
    </div>
  </section>
</template>

<style scoped>
.prbg {
  background: linear-gradient(230.8deg, #aaffd5 0%, #ffffff 100%);
}
</style>
