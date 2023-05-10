<script>
import Item from "./item.vue";
export default {
  components: {
    Item,
  },
  data: () => {
    return {};
  },
  computed: {},
  methods: {},
  mounted() {},
};
</script>

<template>
  <section id="Product">
    <div class="hidden min-[1023px]:block min-[1023px]:relative">
      <div class="top-0 left-0 z-10 triangle"></div>
      <div
        class="min-[1023px]:h-96 xl:h-80 2xl:h-20"
        style="max-height: 500px"
      ></div>
      <div class="absolute z-20 flex top-10">
        <div class="m-10">
          <div class="text-4xl font-semibold text-left">
            {{ $t("poject.Product") }}
          </div>
          <div class="text-left">
            {{ $t("poject.Content1") }}
          </div>
        </div>
        <div>
          <Item />
        </div>
      </div>
    </div>
    <div class="min-[1023px]:hidden pt-10">
      <div class="flex mb-3 min-[781px]:mb-10 max-[782px]:flex-col text-left">
        <h1 class="pl-5 text-3xl font-extrabold">
          {{ $t("poject.Product") }}
        </h1>
        <span
          class="flex items-end justify-center max-[782px]:justify-start pb-1 pl-6 max-[781px]:mt-3"
        >
          {{ $t("poject.Content1") }}
        </span>
      </div>
      <div class="mx-5 border-2 rounded-lg border-violet-700">
        <div class="flex px-8 pt-8">
          <img
            src="@/assets/images/polcker-items-soulwallet.svg"
            alt="soulwallet"
          />
          <h6 class="pl-4 text-3xl font-semibold">SoulWallet</h6>
        </div>
        <div class="px-8 py-5 border-b border-black">
          <p
            class="text-lg text-left xl:text-2xl max-[500px]:text-sm"
            style="font-family: Poppins"
          >
            {{ $t("poject.Content2") }}
          </p>
        </div>
        <div class="px-8 pt-2 text-xl font-semibold text-left">
          <p>{{ $t("poject.Press") }}</p>
        </div>
        <div
          class="flex justify-between px-8 py-5 mb-3 text-lg text-left border-b border-black xl:text-2xl"
        >
          <p class="max-[500px]:text-sm" style="font-family: Poppins">
            {{ $t("poject.Content3") }}
          </p>
          <div class="flex">
            <i data-feather="chevron-right" class="feather-32"> </i>
          </div>
        </div>
        <div class="flex justify-around py-4">
          <a href="https://www.soulwallets.me/" target="_blank">
            <img
              class="mr-5"
              src="@/assets/images/polcker-items-soulwallet-icon.svg"
              alt="iicon"
            />
          </a>
          <a href="https://twitter.com/soulwallet_eth" target="_blank">
            <img
              class="mr-5"
              src="@/assets/images/polcker-items-soulwallet-twitter.svg"
              alt="itwitter"
            />
          </a>
          <a
            href="https://ethglobal.com/showcase/soul-wallet-5srye"
            target="_blank"
          >
            <img
              src="@/assets/images/polcker-items-soulwallet-eth.svg"
              alt="ieth"
            />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.triangle {
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 25vw 50vw 0 0;
  border-color: rgb(171, 255, 213) transparent transparent transparent;
  max-width: 1000px;
  /* background: linear-gradient(180deg, #00FF85 30.84%, rgba(0, 255, 133, 0) 91.06%);
  opacity: 0.1;
  transform: rotate(-180deg); */
}
@media only screen and (min-width: 1444px) {
  .triangle {
    border-width: 500px 600px 0 0;
  }
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
