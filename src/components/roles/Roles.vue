<script>
import feather from "feather-icons";
export default {
  components: {},
  data() {
    return {
      selectrole: "c_member",
    };
  },
  methods: {
    getAanimate(item) {
      this.selectrole = item;
      // console.log("iii", this.$refs);
      // let ttt = Object.keys(this.$refs).filter((v) => {
      //   console.log("xxxx", v);
      //   if (v.indexOf("c_") >= 0) {
      //     console.log("vvv", v);
      //     if (
      //       this.$refs[v].classList.value.indexOf(
      //         "animate__animated animate__bounce animate__backInUp"
      //       ) >= 0
      //     ) {
      //       this.$refs[v].classList.remove(
      //         "animate__animated",
      //         "animate__bounce",
      //         "animate__backInUp"
      //       );
      //     }
      //   }
      // });
      // console.log("ttt", ttt);
      // setTimeout(() => {
      //   this.$refs[item].classList.add(
      //     "animate__animated",
      //     "animate__bounce",
      //     "animate__backInUp"
      //   );
      // }, 500);

      // this.$refs["member"].classList.remove(
      //   "animate__animated",
      //   "animate__backInUp"
      // );
      return "animate__backInUp";
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
  <div class="3xl:container 3xl:mx-auto max-w-screen-3xl rolesbg">
    <div
      class="flex-col px-10 sm:px-24 max-[500px]:px-1 border-green-300 border-y pt-14"
    >
      <p class="pb-5 text-4xl font-semibold">Roles in Plancker</p>
      <p
        class="min-[781px]:px-40 pb-5 text-gray-500"
        style="font-family: Poppins"
      >
        {{ $t("roles.Content1") }}
      </p>
      <div>
        <div
          class="grid items-stretch justify-center grid-flow-col grid-rows-2 min-[781px]:grid-rows-1 max-[500px]:grid-rows-4 pb-10 text-xl font-bold gap-14"
        >
          <div
            class="flex flex-col items-center border rounded-lg justify-center border-b border-[#02FF87] px-10 py-3 bg-white"
            @click="getAanimate('c_observer')"
          >
            <div>
              <img src="@/assets/images/polcker-roles-observer.svg" />
            </div>
            <div class="pt-5">{{ $t("roles.Observer") }}</div>
          </div>
          <div
            class="flex flex-col items-center border rounded-lg justify-center border-[#02FF87] px-10 py-3 bg-white"
            @click="getAanimate('c_member')"
          >
            <div>
              <img src="@/assets/images/polcker-roles-general.svg" />
            </div>
            <div class="pt-5">{{ $t("roles.Member") }}</div>
          </div>
          <div
            class="flex flex-col items-center border rounded-lg justify-center border-[#02FF87] px-10 py-3 bg-white"
            @click="getAanimate('c_corebuilder')"
          >
            <div>
              <img src="@/assets/images/polcker-roles-corebuilder.svg" />
            </div>
            <div class="pt-5">{{ $t("roles.CoreBuilder") }}</div>
          </div>
          <div
            class="flex flex-col items-center border rounded-lg justify-center border-[#02FF87] px-10 py-3 bg-white"
            @click="getAanimate('c_corecontributor')"
          >
            <div>
              <img src="@/assets/images/polcker-roles-corecontribution.svg" />
            </div>
            <div class="pt-5">{{ $t("roles.CoreContributor") }}</div>
          </div>
        </div>
      </div>
    </div>
    <div
      v-if="selectrole == 'c_observer'"
      ref="c_observer"
      class="flex-col px-10 sm:px-24 max-[500px]:px-1 border-green-300 pt-14"
    >
      <p class="text-4xl font-semibold">
        {{ $t("roles.HowToBe") }} {{ $t("roles.Observer") }}
      </p>
      <div>
        <div
          class="flex flex-col my-10 px-10 sm:px-24 max-[500px]:px-1 text-white"
        >
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.ObserverObject.Bar1") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.ObserverObject.Bar2") }}
          </div>
        </div>
      </div>
    </div>
    <div
      v-if="selectrole == 'c_member'"
      ref="c_member"
      class="flex-col px-10 sm:px-24 max-[500px]:px-1 border-green-300 pt-14"
    >
      <p class="text-4xl font-semibold">
        {{ $t("roles.HowToBe") }} {{ $t("roles.Member") }}
      </p>
      <div>
        <div
          class="max-[781px]:hidden grid grid-cols-1 min-[781px]:grid-cols-10 gap-1 my-10 font-mono text-sm font-bold leading-6 text-center text-white min-[781px]:mx-28 auto-cols-max"
        >
          <div
            class="min-[781px]:col-span-3 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar1") }}
          </div>
          <div
            class="col-span-3 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar2") }}
          </div>
          <div
            class="col-span-4 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar3") }}
          </div>
          <div class="col-span-2 p-4 bg-indigo-500 shadow-lg">
            {{ $t("roles.MemberObject.Bar4") }}
          </div>
          <div
            class="col-span-6 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar5") }}
          </div>
          <div
            class="col-span-6 min-[781px]:col-span-2 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar6") }}
          </div>
          <div
            class="col-span-6 min-[781px]:col-span-5 p-4 bg-indigo-500 shadow-lg"
          >
            {{ $t("roles.MemberObject.Bar7") }}
          </div>
          <div
            class="col-span-6 min-[781px]:col-span-5 p-4 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar8") }}
          </div>
        </div>
        <div class="flex flex-col min-[781px]:hidden py-5 text-white">
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar1") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar2") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar3") }}
          </div>
          <div class="p-4 mb-1 bg-indigo-500 shadow-lg">
            {{ $t("roles.MemberObject.Bar4") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar5") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar6") }}
          </div>
          <div class="p-4 mb-1 bg-indigo-500 shadow-lg">
            {{ $t("roles.MemberObject.Bar7") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.MemberObject.Bar8") }}
          </div>
        </div>
      </div>
    </div>
    <div
      v-if="selectrole == 'c_corebuilder'"
      ref="c_corebuilder"
      class="flex-col px-10 sm:px-24 max-[500px]:px-1 border-green-300 pt-14"
    >
      <p class="text-4xl font-semibold">
        {{ $t("roles.HowToBe") }} {{ $t("roles.CoreBuilder") }}
      </p>
      <div>
        <div
          class="flex flex-col my-10 px-10 sm:px-24 max-[500px]:px-1 text-white"
        >
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar1") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar2") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar3") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar4") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar5") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar6") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreBuilderObject.Bar7") }}
          </div>
        </div>
      </div>
    </div>
    <div
      v-if="selectrole == 'c_corecontributor'"
      ref="c_corecontributor"
      class="flex-col px-10 sm:px-24 max-[500px]:px-1 border-green-300 pt-14"
    >
      <p class="text-4xl font-semibold">
        {{ $t("roles.HowToBe") }} {{ $t("roles.CoreContributor") }}
      </p>
      <div>
        <div
          class="flex flex-col my-10 px-10 sm:px-24 max-[500px]:px-1 text-white"
        >
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreObject.Bar1") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreObject.Bar2") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreObject.Bar3") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-500 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreObject.Bar4") }}
          </div>
          <div
            class="p-4 mb-1 bg-indigo-300 dark:bg-indigo-800 dark:text-indigo-400"
          >
            {{ $t("roles.CoreObject.Bar5") }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.rolesbg {
  background: linear-gradient(180.86deg, #b0ffd8 -8.22%, #ffffff 111.63%);
}
</style>
