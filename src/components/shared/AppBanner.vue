<script>
import feather from "feather-icons";

export default {
  name: "Home",
  data: () => {
    return {
      theme: "",
      placeholder: true,
    };
  },
  created() {
    this.theme = localStorage.getItem("theme") || "light";
  },
  mounted() {
    feather.replace();
    this.theme = localStorage.getItem("theme") || "light";
  },
  updated() {
    feather.replace();
  },
  methods: {
    isLoad() {
      this.placeholder = false;
    },
  },
};
</script>

<template>
  <section class="relative">
    <div class="relative pr-5">
      <div v-if="placeholder" class="w-full placeholder">
        <div class="animated-background"></div>
      </div>
      <img
        @load="isLoad"
        class="xl:w-full"
        src="@/assets/images/plocker-banner.svg"
        alt="banner"
      />
      <div
        v-if="!placeholder"
        class="absolute w-3/6 p-1 left-8 top-7 w-12/12 sm:w-8/12 sm:top-0 lg:w-7/12 md:top-12"
      >
        <p
          class="mb-5 text-xl font-bold tracking-widest text-left sm:text-4xl lg:text-6xl max-[430px]:text-sm"
          style="line-height: 1.5"
        >
          {{ $t("banner.Title") }}
        </p>
      </div>
      <router-link to="/joinus">
        <div
          v-if="!placeholder"
          class="absolute flex p-2 font-bold text-black border border-black rounded-lg right-7 w-36 justify-evenly top-10 md:top-16 lg:right-10 sm:top-5 max-[430px]:text-sm max-[430px]:p-1 max-[430px]:w-28"
        >
          <p>{{ $t("banner.Onboarding") }}</p>
          <i
            data-feather="chevron-right"
            class="text-liText-ternary-dark hover:text-gray-400"
          ></i>
        </div>
      </router-link>
      <div
        v-if="!placeholder"
        class="absolute flex justify-between w-48 text-white ml-14 max-[781px]:ml-10 bottom-5"
      >
        <a href="https://plancker.notion.site/" target="_blank">
          <img
            class="max-[781px]:h-5 max-[781px]:w-5"
            src="@/assets/images/plocker-banner-notion.svg"
            alt="notion"
          />
        </a>
        <a href="https://twitter.com/PlanckerDao" target="_blank"
          ><img
            class="max-[781px]:h-5 max-[781px]:w-5"
            src="@/assets/images/plocker-banner-twitter.svg"
            alt="twitter"
        /></a>
        <a href="https://discord.com/invite/v59KDSgqFu" target="_blank">
          <img
            class="max-[781px]:h-5 max-[781px]:w-5"
            src="@/assets/images/plocker-banner-discord.svg"
            alt="discord"
          />
        </a>
        <a href="https://forum.plancker.org/" target="_blank">
          <img
            class="max-[781px]:h-5 max-[781px]:w-5"
            src="@/assets/images/plocker-banner-f.svg"
            alt="f"
          />
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
.placeholder {
  margin: 0 auto;
  /* max-width: 200px;*/
  min-height: 300px;
  background-color: #eee;
}

@keyframes placeHolderShimmer {
  0% {
    background-position: -468px 0;
  }
  100% {
    background-position: 468px 0;
  }
}

.animated-background {
  animation-duration: 1.25s;
  animation-fill-mode: forwards;
  animation-iteration-count: infinite;
  animation-name: placeHolderShimmer;
  animation-timing-function: linear;
  background: darkgray;
  background: linear-gradient(to right, #eeeeee 10%, #dddddd 18%, #eeeeee 33%);
  background-size: 800px 104px;
  height: 400px;
  position: relative;
}
</style>
