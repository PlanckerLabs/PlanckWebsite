<script>
import AppBanner from "@/components/shared/AppBanner";

import PublicLayoutGrid from "../components/publiclayer/PublicLayoutGrid.vue";
import ProgressBar from "../components/progressbar/ProgressBar.vue";
import Items from "../components/items/Items.vue";
import PublicPool from "../components/publicpool/PublicPool.vue";
import PreResearch from "../components/preresearch/PreResearch.vue";
export default {
  name: "Home",
  components: {
    AppBanner,
    PublicLayoutGrid,
    ProgressBar,
    Items,
    PublicPool,
    PreResearch,
  },
};
</script>

<template>
  <div class="2xl:container 2xl:mx-auto max-w-screen-2xl">
    <!-- Banner -->
    <AppBanner class="mb-5 sm:mb-8" />
    <!-- Public Layer -->
    <PublicLayoutGrid />
    <ProgressBar />
    <div
      style="
        background: linear-gradient(180deg, #d2cdff 0%, #daffec 100.67%);
        /* opacity: 0.67; */
      "
    >
      <Items />
      <PublicPool />
      <PreResearch />
    </div>
  </div>
</template>

<style scoped></style>
