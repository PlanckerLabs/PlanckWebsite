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
  <section id="Partner">
    <div class="2xl:container 2xl:mx-auto max-w-screen-2xl">
      <div
        class="hidden pt-10 pb-8 text-white bg-black border-t-2 min-[781px]:flex min-[781px]:flex-col"
      >
        <div
          class="grid items-center justify-center grid-flow-col grid-rows-1 pb-10 text-xl border-b-2 gap-11 border-slate-600"
        >
          <div class="flex">
            <img src="@/assets/images/polcker-footer-icon.svg" alt="polcker" />
            <p class="pl-2">{{ $t("footer.Partners") }}</p>
          </div>
          <div class="flex">
            <img
              src="@/assets/images/polcker-footer-greenPill.svg"
              alt="greePill"
            />
            <p class="pl-2">GreenPill CN</p>
          </div>
          <div class="flex">
            <img src="@/assets/images/polcker-footer-four.svg" alt="4 SEAS" />
            <p class="pl-2">{{ $t("footer.Seas") }}</p>
          </div>
          <div class="flex">
            <p>GCC Eco</p>
          </div>
          <div class="flex">
            <p>LxDao</p>
          </div>
        </div>
        <div
          class="grid items-start justify-center grid-flow-col grid-rows-1 gap-20 mt-10 text-xl text-left"
        >
          <div class="flex-col">
            <h6 class="mb-5 font-extrabold">{{ $t("footer.Follow") }}</h6>
            <ul class="text-lg" style="line-height: 2em">
              <li>
                <a href="https://t.me/planckeropencommunity" target="_blank"
                  >Telegram</a
                >
              </li>
              <li>
                <a href="https://twitter.com/PlanckerDao" target="_blank"
                  >Twitter</a
                >
              </li>
              <li>
                <a href="https://discord.com/invite/v59KDSgqFu" target="_blank"
                  >Discord</a
                >
              </li>
              <li>
                <a href="https://mirror.xyz/plancker.eth" target="_blank"
                  >Mirror</a
                >
              </li>
            </ul>
          </div>
          <div class="flex-col">
            <h6 class="mb-5 font-extrabold">{{ $t("footer.Govern") }}</h6>
            <ul class="text-lg" style="line-height: 2em">
              <li>
                <a href="https://plancker.notion.site/" target="_blank"
                  >Notion</a
                >
              </li>
              <li>
                <a href="https://forum.plancker.org/" target="_blank">Forum</a>
              </li>
              <li>SOP</li>
            </ul>
          </div>
          <div class="flex-col">
            <h6 class="mb-5 font-extrabold">
              {{ $t("footer.AboutPlancker") }}
            </h6>
            <ul class="text-lg">
              <li>
                <p style="padding-top: 5px; width: 34rem">
                  {{ $t("footer.Content") }}
                </p>
              </li>
              <li style="line-height: 4em">
                <router-link to="/joinus">{{
                  $t("footer.Onboarding")
                }}</router-link>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="min-[781px]:hidden">
      <div class="text-white bg-black max-[500px]:text-sm">
        <div class="flex justify-center py-5">
          <img src="@/assets/images/polcker-footer-icon.svg" alt="polcker" />
          <p class="pl-2">{{ $t("footer.Partners") }}</p>
        </div>
        <div
          class="grid justify-center grid-flow-col grid-rows-1 py-10 text-xl border-b-2 gap-11 border-slate-600 max-[500px]:gap-5 max-[500px]:text-sm"
        >
          <div class="flex">
            <img
              src="@/assets/images/polcker-footer-greenPill.svg"
              alt="greePill"
            />
            <p class="pl-2">GreenPill CN</p>
          </div>
          <div class="flex">
            <img src="@/assets/images/polcker-footer-four.svg" alt="4 SEAS" />
            <p class="pl-2">{{ $t("footer.Seas") }}</p>
          </div>
          <div class="flex">
            <p>GCC Eco</p>
          </div>
          <div class="flex">
            <p>LxDao</p>
          </div>
        </div>
        <div
          class="grid items-center justify-center grid-flow-col grid-rows-1 py-10 text-xl border-b-2 gap-11 border-slate-600 max-[500px]:gap-5 max-[500px]:text-sm"
        >
          <div class="flex">
            <p>{{ $t("footer.Follow") }} :</p>
          </div>
          <div class="flex">
            <a href="https://t.me/planckeropencommunity" target="_blank">
              <img
                src="@/assets/images/polcker-footer-telegram.svg"
                alt="telegram"
              />
            </a>
          </div>
          <div class="flex">
            <a href="https://twitter.com/PlanckerDao" target="_blank">
              <img
                src="@/assets/images/polcker-footer-twitter.svg"
                alt="twitter"
              />
            </a>
          </div>
          <div class="flex">
            <a href="https://discord.com/invite/v59KDSgqFu" target="_blank">
              <img
                src="@/assets/images/polcker-footer-discord.svg"
                alt="discord"
              />
            </a>
          </div>
          <div class="flex">
            <a href="https://mirror.xyz/plancker.eth" target="_blank">
              <img
                src="@/assets/images/polcker-footer-mirror.svg"
                alt="mirror"
              />
            </a>
          </div>
        </div>
        <div
          class="grid items-center justify-center grid-flow-col grid-rows-1 py-10 text-xl border-b-2 gap-11 border-slate-600 max-[500px]:gap-5 max-[500px]:text-sm"
        >
          <div class="flex">
            <p>{{ $t("footer.Govern") }} :</p>
          </div>
          <div class="flex">
            <a href="https://plancker.notion.site/" target="_blank">
              <img
                src="@/assets/images/polcker-footer-notion.svg"
                alt="notion"
              />
            </a>
          </div>
        </div>
        <div
          class="grid items-start justify-center grid-flow-col grid-rows-1 gap-20 mt-10 text-xl text-center max-[500px]:text-sm"
        >
          <div class="flex-col">
            <h6 class="mb-5 font-extrabold">
              {{ $t("footer.AboutPlancker") }}
            </h6>
            <ul class="text-lg max-[500px]:text-sm">
              <li>
                <p style="padding-top: 5px; width: 34rem">
                  {{ $t("footer.Content") }}
                </p>
              </li>
              <li class="flex justify-center h-10 py-3">
                <router-link to="/joinus">
                  <div
                    class="flex items-center p-2 font-bold text-white border border-white rounded-lg right-7 w-36 justify-evenly top-10 md:top-16 lg:right-10 sm:top-5"
                  >
                    <p>{{ $t("footer.Onboarding") }}</p>
                    <i
                      data-feather="chevron-right"
                      class="text-liText-ternary-dark hover:text-gray-400"
                    ></i>
                  </div>
                </router-link>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
