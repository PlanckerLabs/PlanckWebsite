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
    <div class="px-5 pt-20">
      <p class="mb-5 text-3xl font-semibold">
        Plancker <sup class="font-bold text-green-400">^</sup>
        {{ $t("dework.PlanckerMap") }}
      </p>
      <div class="flex items-center justify-center">
        <img
          class="p-2 rounded-lg"
          src="@/assets/images/project_map.png"
          alt="map"
        />
      </div>
      <div>
        <div class="mt-10">
          <p class="pb-3 font-semibold text-left whitespace-normal">
            {{ $t("dework.Title1") }}
          </p>
        </div>
        <div class="text-left">
          <ul
            class="list-outside"
            style="display: block; list-style-type: none; margin: 3px"
          >
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title1_Item1") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title1_Item2") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title1_Item3") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title1_Item4") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title1_Item5") }}
            </li>
          </ul>
        </div>
      </div>

      <div class="py-10">
        <div class="pb-3">
          <p class="font-semibold text-left whitespace-normal">
            {{ $t("dework.Title2") }}
          </p>
        </div>
        <div class="text-left">
          <ul
            class="list-outside"
            style="display: block; list-style-type: none; margin: 3px"
          >
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title2_Item1") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title2_Item2") }}
            </li>
            <li class="pl-5 mb-2 border-l-4 border-l-green-300">
              {{ $t("dework.Title2_Item3") }}
            </li>
          </ul>
        </div>
      </div>

      <div>
        <p class="text-left whitespace-normal"></p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
