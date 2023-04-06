<script>
export default {
  components: {},
  data: () => {
    return {};
  },
  computed: {},
  methods: {},
  mounted() {},
};
</script>

<template>
  <!-- Projects grid -->
  <section
    id="PublicLayer"
    class="px-5 pt-10 pb-5 sm:pt-14"
    style="
      background: rgb(0, 255, 133);
      background: linear-gradient(
        180deg,
        rgba(0, 0, 0, 0) 0%,
        rgba(0, 255, 133, 0.1) 62%,
        rgba(0, 255, 133, 0.1) 100%
      );
    "
  >
    <div class="flex mb-3 max-[782px]:flex-col text-left min-[781px]:mb-10">
      <h1 class="min-[781px]:pl-5 text-3xl font-extrabold">
        {{ $t("publiclayer.Publiclayer") }}
      </h1>
      <span
        class="flex items-end justify-center pb-1 min-[781px]:pl-6 max-[781px]:mt-3"
      >
        {{ $t("publiclayer.Content1") }}
      </span>
    </div>
    <div class="hidden min-[781px]:flex">
      <div
        class="group content-around w-1/3 h-auto py-8 border border-gray-500 rounded-lg px-14 cardg hover:border-[#02FF87]"
      >
        <a
          href="https://plancker.notion.site/V-For-V_Cult-V-d19319a531a147bf84f07a1deb0b9ee4"
          target="_blank"
        >
          <div class="flex items-center pb-5 text-2xl font-bold border-b">
            <img
              class="z-10"
              src="@/assets/images/polcker-publiclayout-book.svg"
              alt="book"
            />
            <p class="ml-5">{{ $t("publiclayer.VForVCult") }}</p>
            <i data-feather="chevron-right" class="group-hover:text-green-400">
            </i>
          </div>
          <div class="pt-10 text-lg text-left">
            <p style="font-family: Poppins">
              {{ $t("publiclayer.Content2") }}
            </p>
          </div>
        </a>
      </div>

      <div class="flex-col justify-between w-2/3 ml-5">
        <a
          class="flex"
          href="https://plancker.notion.site/Great-China-Community-Eco-9003584d04a74a488daacac32838c8c8"
          target="_blank"
        >
          <div
            class="flex items-center h-1/2 border border-gray-500 rounded-lg py-7 px-8 cardg hover:border-[#02FF87]"
          >
            <div class="flex items-center w-5/12 h-full max-[1130px]:flex-col">
              <div class="max-[1130px]:pb-5">
                <img
                  src="@/assets/images/polcker-publiclayout-group.svg"
                  alt="group"
                />
              </div>
              <div class="pl-10 text-2xl font-bold text-left">
                <p>{{ $t("publiclayer.Eco1") }}</p>
                <p>{{ $t("publiclayer.Eco2") }}</p>
              </div>
            </div>
            <div class="w-7/12 py-2 pl-8 text-left border-l">
              <p style="font-family: Poppins">
                {{ $t("publiclayer.Content3") }}
              </p>
            </div>
          </div>
        </a>
        <div
          class="flex items-center border border-gray-500 rounded-lg py-7 px-8 cardg hover:border-[#02FF87] mt-3.5"
        >
          <a
            class="flex"
            href="https://plancker.notion.site/Daostar-e1bfdbef25ca466589932b0eeb98c3b0"
            target="_blank"
          >
            <div
              class="flex items-center w-5/12 h-full border-r py-7 max-[1130px]:flex-col"
            >
              <div class="max-[1130px]:pb-5">
                <img
                  src="@/assets/images/polcker-publiclayout-doastart.svg"
                  alt="doastart"
                />
              </div>
              <div class="pl-10 text-2xl font-bold text-left">
                <p>{{ $t("publiclayer.Daostar1") }}</p>
                <p>{{ $t("publiclayer.Daostar2") }}</p>
              </div>
            </div>
            <div class="w-7/12 py-2 pl-8 text-left border-l">
              <p style="font-family: Poppins">
                {{ $t("publiclayer.Content4") }}
              </p>
            </div>
          </a>
        </div>
      </div>
    </div>
    <!-- < 781 -->
    <div class="flex flex-col min-[781px]:hidden">
      <div
        class="group content-around h-auto py-5 mb-5 border border-gray-500 rounded-lg px-5 cardg hover:border-[#02FF87]"
      >
        <div
          class="flex items-center justify-between pb-5 text-2xl font-bold border-b"
        >
          <div class="flex items-center">
            <img
              class="w-16 h-16"
              src="@/assets/images/polcker-publiclayout-book.svg"
              alt="book"
            />
            <p class="ml-5">{{ $t("publiclayer.VForVCult") }}</p>
          </div>
          <div class="flex">
            <i data-feather="chevron-right" class="text-green-400 feather-32">
            </i>
          </div>
        </div>
        <div class="pt-10 text-lg text-left">
          <p class="max-[500px]:text-sm" style="font-family: Poppins">
            {{ $t("publiclayer.Content2") }}
          </p>
        </div>
      </div>
      <div
        class="group content-around h-auto py-5 mb-5 border border-gray-500 rounded-lg px-5 cardg hover:border-[#02FF87]"
      >
        <div class="flex pb-5 text-2xl font-bold border-b">
          <a
            class="flex items-center justify-between w-full"
            href="https://plancker.notion.site/Great-China-Community-Eco-9003584d04a74a488daacac32838c8c8"
            target="_blank"
          >
            <div class="flex items-center">
              <img
                class="w-16 h-16"
                src="@/assets/images/polcker-publiclayout-group.svg"
                alt="book"
              />
              <p class="ml-5">
                {{ $t("publiclayer.Eco1") }}{{ $t("publiclayer.Eco2") }}
              </p>
            </div>
            <div class="flex">
              <i data-feather="chevron-right" class="text-green-400 feather-32">
              </i>
            </div>
          </a>
        </div>
        <div class="pt-10 text-lg text-left">
          <p class="max-[500px]:text-sm" style="font-family: Poppins">
            {{ $t("publiclayer.Content3") }}
          </p>
        </div>
      </div>
      <div
        class="group content-around h-auto py-5 mb-5 border border-gray-500 rounded-lg px-5 cardg hover:border-[#02FF87]"
      >
        <div
          class="flex items-center justify-between pb-5 text-2xl font-bold border-b"
        >
          <div class="flex items-center">
            <img
              class="w-16 h-16"
              src="@/assets/images/polcker-publiclayout-doastart.svg"
              alt="doastart"
            />
            <p class="ml-5">
              {{ $t("publiclayer.Daostar1") }}{{ $t("publiclayer.Daostar2") }}
            </p>
          </div>
          <div class="flex">
            <i data-feather="chevron-right" class="text-green-400 feather-32">
            </i>
          </div>
        </div>
        <div class="pt-10 text-lg text-left">
          <p class="max-[500px]:text-sm" style="font-family: Poppins">
            {{ $t("publiclayer.Content4") }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.cardg {
  background: linear-gradient(
    221.15deg,
    #aaffd5 0%,
    rgba(255, 255, 255, 0) 94.25%
  );
}
.feather-16 {
  width: 16px;
  height: 16px;
}

.feather-24 {
  width: 24px;
  height: 24px;
}

.feather-32 {
  font-weight: 800;
  width: 32px;
  height: 32px;
}
</style>
