<script>
export default {
  props: ["showModal", "isOpen"],
};
</script>

<template>
  <!-- Header links -->
  <div
    :class="isOpen ? 'block' : 'hidden'"
    class="flex-col items-center justify-end p-5 m-0 mt-5 shadow-lg sm:flex sm:flex-row sm:ml-4 sm:mt-3 sm:p-0 sm:shadow-none md:w-2/3"
  >
    <router-link
      :to="{ hash: '#PublicLayer' }"
      class="block mb-2 text-lg font-semibold text-left font-general-medium text-primary-dark border-b-4 border-[#0CFF8A] sm:mx-4 sm:py-2 xl:mx-8"
      aria-label="Projects"
      >{{ $t("navigation.PublicLayer") }}</router-link
    >
    <router-link
      :to="{ hash: '#Product' }"
      class="block pt-3 mb-2 text-lg font-semibold text-left border-t-2 border-b-4 border-b-white font-general-medium text-primary-dark sm:mx-4 sm:py-2 sm:pt-2 sm:border-t-0 border-primary-light xl:mx-8"
      aria-label="About Me"
      >{{ $t("navigation.Product") }}</router-link
    >
    <router-link
      :to="{ hash: '#PublicPool' }"
      class="block pt-3 mb-2 text-lg font-semibold text-left border-t-2 border-b-4 font-general-medium text-primary-dark sm:mx-4 border-b-white sm:py-2 sm:pt-2 sm:border-t-0 border-primary-light xl:mx-8"
      aria-label="Contact"
      >{{ $t("navigation.PublicPool") }}</router-link
    >
    <router-link
      :to="{ hash: '#Research' }"
      class="block pt-3 mb-2 text-lg font-semibold text-left border-t-2 border-b-4 font-general-medium text-primary-dark sm:mx-4 border-b-white sm:py-2 sm:pt-2 sm:border-t-0 border-primary-light xl:mx-8"
      aria-label="Contact"
      >{{ $t("navigation.Pre-Research") }}</router-link
    >
    <router-link
      :to="{ hash: '#Partner' }"
      class="block pt-3 mb-2 text-lg font-semibold text-left border-t-2 border-b-4 font-general-medium text-primary-dark sm:mx-4 border-b-white sm:py-2 sm:pt-2 sm:border-t-0 border-primary-light xl:mx-8"
      aria-label="Contact"
      >{{ $t("navigation.Partner") }}</router-link
    >
  </div>
</template>

<style lang="scss" scoped></style>
