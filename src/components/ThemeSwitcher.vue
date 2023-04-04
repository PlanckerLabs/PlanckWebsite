<script>
import feather from "feather-icons";
export default {
  props: {
    theme: {
      type: String,
      required: true,
    },
  },
  methods: {
    toggleTheme() {
      const newTheme = this.theme === "light" ? "dark" : "light";
      localStorage.setItem("theme", newTheme);
      this.$emit("theme-changed", newTheme);
      this.$router.go();
    },
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
  <a
    v-if="$i18n.locale == 'cn'"
    class="flex"
    href="#"
    @click="$i18n.locale = 'en'"
  >
    <i data-feather="globe" class="hover:text-gray-400"> </i>
    <p class="pl-1 font-semibold">中</p>
  </a>
  <a
    v-if="$i18n.locale == 'en'"
    class="flex"
    href="#"
    @click="$i18n.locale = 'cn'"
  >
    <i data-feather="globe" class="hover:text-gray-400"> </i>
    <p class="pl-1 font-semibold">EN</p>
  </a>
</template>
