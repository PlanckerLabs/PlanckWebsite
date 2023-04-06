<script>
import ThemeSwitcher from "../ThemeSwitcher";

import feather from "feather-icons";
import AppHeaderLinks from "./AppHeaderLinks.vue";

export default {
  components: {
    ThemeSwitcher,
    AppHeaderLinks,
  },
  data() {
    return {
      isOpen: false,
      theme: "",
      modal: false,
    };
  },

  created() {
    this.theme = localStorage.getItem("theme") || "light";
  },
  mounted() {
    feather.replace();
    this.theme = localStorage.getItem("theme") || "light";
  },
  methods: {
    updateTheme(theme) {
      this.theme = theme;
    },
  },
  updated() {
    feather.replace();
  },
};
</script>

<template>
  <section
    id="nav"
    class="min-[500px]:mx-10 2xl:container 2xl:mx-auto max-w-screen-2xl"
  >
    <!-- Header start -->
    <div class="z-10 block mt-6 sm:flex sm:justify-between sm:items-center">
      <!-- Header menu links and small screen hamburger menu -->
      <div class="flex items-center justify-between px-4 sm:px-0">
        <!-- Header logos -->
        <div>
          <router-link to="/">
            <img
              src="@/assets/images/plocker-logo-light.svg"
              class="w-36"
              alt="Light Logo"
            />
          </router-link>
        </div>

        <!-- Theme switcher small screen -->
        <div
          class="sm:hidden bg-ternary-light dark:bg-ternary-dark hover:bg-hover-light hover:shadow-sm px-2.5 py-2 rounded-lg"
        >
          <theme-switcher :theme="theme" @themeChanged="updateTheme" />
        </div>

        <!-- Small screen hamburger menu -->
        <div class="sm:hidden">
          <button
            @click="isOpen = !isOpen"
            type="button"
            class="focus:outline-none"
            aria-label="Hamburger Menu"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              class="fill-current h-7 w-7 text-secondary-dark dark:text-ternary-light"
            >
              <path
                v-if="isOpen"
                fill-rule="evenodd"
                d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
                clip-rule="evenodd"
              ></path>
              <path
                v-if="!isOpen"
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>

      <!-- Header links -->
      <AppHeaderLinks :isOpen="isOpen" />

      <!-- Header right section buttons -->
      <div
        class="flex-col items-center justify-between hidden sm:flex md:flex-row"
      >
        <!-- Theme switcher large screen -->
        <theme-switcher
          :theme="theme"
          @themeChanged="updateTheme"
          class="px-3 py-2 ml-8 shadow-sm cursor-pointer bg-primary-light dark:bg-ternary-dark rounded-xl"
        />
      </div>
    </div>
  </section>
</template>

<style scoped>
#nav a.router-link-exact-active {
  @apply text-indigo-700;
  @apply dark:text-indigo-400;
  @apply font-medium;
}
</style>
