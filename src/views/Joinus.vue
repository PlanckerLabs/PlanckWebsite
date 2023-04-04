<script>
import DeWork from "../components/dework/DeWork.vue";
import PlanckerMap from "../components/planckermap/PlanckerMap.vue";
import Roles from "../components/roles/Roles.vue";
import Calendar from "../components/calendar/calendar.vue";
import "animate.css";

export default {
  name: "Joinus",
  components: {
    DeWork,
    PlanckerMap,
    Roles,
    Calendar,
  },
};
</script>

<template>
  <div class="2xl:container 2xl:mx-auto max-w-screen-2xl">
    <div class="mx-10 border border-green-300 max-[500px]:mx-3">
      <DeWork />
      <PlanckerMap />
      <Roles />
    </div>
    <Calendar />
  </div>
</template>

<style scoped></style>
