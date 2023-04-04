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
  <div class="p-8 mr-5 border rounded-lg itembg">
    <div class="flex">
      <img
        src="@/assets/images/polcker-items-soulwallet.svg"
        alt="soulwallet"
      />
      <h6 class="pl-4 text-3xl font-semibold">SoulWallet</h6>
    </div>
    <div class="pt-5 pr-2">
      <p class="text-lg text-left xl:text-2xl" style="font-family: Poppins">
        {{ $t("poject.Content2") }}
      </p>
    </div>
    <div class="pt-10 text-xl font-semibold text-left">
      <p>{{ $t("poject.Press") }}</p>
    </div>
    <div class="w-2/3 pt-1 text-lg text-left mb-7 xl:text-2xl">
      <p
        style="font-family: Poppins"
        class="leading-10 underline underline-offset-8 decoration-4 decoration-green-300"
      >
        {{ $t("poject.Content3") }}
      </p>
    </div>
    <div class="flex px-1 py-10">
      <div
        class="flex items-center justify-around w-2/3 text-lg xl:text-2xl md:text-sm"
      >
        <div>{{ $t("poject.Contributor") }}</div>
        <div class="flex items-center">
          <a
            class="flex items-center"
            href="https://twitter.com/zengjiajun_eth"
            target="_blank"
          >
            <img src="@/assets/images/polcker-items-cer3.svg" alt="cer3" />
            <p class="pl-3">JiaJun</p>
          </a>
        </div>
        <div>
          <a
            class="flex items-center"
            href="https://twitter.com/jhfnetboy"
            target="_blank"
          >
            <img src="@/assets/images/polcker-items-cer2.svg" alt="cer2" />
            <p class="pl-3">Jhfnetboy</p>
          </a>
        </div>
        <div>
          <a
            class="flex items-center"
            href="https://twitter.com/cejay519"
            target="_blank"
          >
            <img src="@/assets/images/polcker-items-cer1.svg" alt="cer1" />
            <p class="pl-3">Cejay</p>
          </a>
        </div>
      </div>
      <div class="flex justify-end w-1/3">
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
</template>

<style scoped>
.itembg {
  background: linear-gradient(103.17deg, #ffffff -2.98%, #a39bff 115.37%);
  border: 1px solid #544dff;
  border-radius: 10px;
}
</style>
