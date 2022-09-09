<template>
  <div>
    <head-page></head-page>
    <div class="rd-left">
      <img class="rd-green" src="@/assets/circle-green.png" />
      <img class="rd-orange-sm" src="@/assets/orange-sm.png" />
      <img class="rd-green-sm" src="@/assets/green-sm.png" />
    </div>
    <div class="rd-right justify-content-end">
      <img class="rd-white" src="@/assets/circle-white.png" />
      <img class="rd-orange-fill" src="@/assets/orange-fill.png" />
      <img class="rd-orange-bg" src="@/assets/orange-bg.png" />
    </div>
  </div>
</template>

<script>
import HeadPage from "./HeadPage.vue";

export default {
  name: "HeadPageCircle",
  components: {
    HeadPage,
  },
};
</script>

<style>
@media only screen and (max-width: 1000px) {
  .rd-left, .rd-right {
    display: none;
  }
}
.head-page {
  position: relative;
}
.rd-left {
  position: absolute;
  top: 0;
}
.rd-right {
  position: relative;
  margin-top: -45% !important;
}
.rd-green {
  margin-left: -30% !important;
  margin-top: 140% !important;
}
.rd-orange-sm {
  margin-left: 10% !important;
}
.rd-green-sm {
  margin-left: -9% !important;
  margin-top: 80% !important;
}
.rd-orange-bg {
  margin-left: 90% !important;
  margin-top: -40% !important;
}
.rd-orange-fill {
  margin-left: 60% !important;
  margin-top: -40% !important;
}
.rd-white {
  margin-top: 13% !important;
  margin-left: 51% !important;
}
</style>
