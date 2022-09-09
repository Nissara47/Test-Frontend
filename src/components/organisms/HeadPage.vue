<template>
  <div>
    <div>
      <img class="yellow-bg w-100" src="@/assets/circle.png" />
    </div>
    <div class="row justify-content-center align-content-start content w-100">
      <img class="body-ant" src="@/assets/ant3.png" />
      <img class="head-ant" src="@/assets/ant2.png" />
      <molecule-input class="input-form col-lg-4 col-md-8 col-sm-8"></molecule-input>
      <img class="pic-people col-lg-8 col-md-4 align-self-end" src="@/assets/people.png" />
    </div>
  </div>
</template>

<script>
import MoleculeInput from "../molecules/MoleculeInput.vue";
export default {
  name: "HeadPage",
  components: {
    MoleculeInput,
  },
};
</script>
<style scoped>
@media only screen and (max-width: 1100px) {
  .pic-people {
    display: none;
  }
}
@media only screen and (max-width: 299px) {
  .head-ant, .body-ant {
    display: none;
  }
  .input-form {
    margin-top: 100px !important;
  }
}
@media only screen and (min-width: 300px) and (max-width: 550px) {
  .head-ant, .body-ant {
    display: none;
  }
  .input-form {
    margin-top: 125px !important;
  }
}
@media only screen and (min-width: 551px) and (max-width: 950px) {
  .head-ant, .body-ant {
    display: none;
  }
}
.head-ant {
  margin-top: 4vh !important;
  margin-right: -4vh !important;
  width: 12vh;
  height: 10vh;
}
.body-ant {
  margin-top: 10vh !important;
  margin-right: -12vh !important;
  width: 10vh;
  height: 6vh;
}
.yellow-bg {
  position: relative;
}
.content {
  position: absolute;
  top: 9%;
}
.pic-people {
  width: 40% !important;
  height: 40% !important;
  margin-left: 3% !important;
}
</style>
