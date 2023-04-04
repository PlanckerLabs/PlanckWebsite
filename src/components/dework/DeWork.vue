<script>
import feather from "feather-icons";
export default {
  components: {},
  data() {
    return {};
  },
  mounted() {
    feather.replace();
  },
  updated() {
    feather.replace();
  },
};
</script>

<template>
  <div class="3xl:container 3xl:mx-auto max-w-screen-3xl">
    <div
      class="flex-col w-full h-72 pt-16 text-black bg-[#00FF85] bg-cover bg-[url('@/assets/images/polcker-dework-banner.svg')]"
    >
      <p class="mb-5 text-4xl xl:text-6xl font-semibold max-[500px]:text-lg">
        {{ $t("dework.Onboarding") }}
      </p>
      <p class="mb-5 text-2xl xl:text-4xl font-bold max-[500px]:text-lg">
        {{ $t("dework.Create") }}
      </p>
      <div class="flex items-center justify-center">
        <a href="https://app.dework.xyz/plancker-dao" target="_blank">
          <div
            class="flex p-2 text-black border border-black rounded-lg w-36 justify-evenly"
          >
            <p>{{ $t("dework.Dework") }}</p>
            <i data-feather="chevron-right"></i>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
