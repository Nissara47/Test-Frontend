<template>
  <div>
    <div class="head">
      <head-page-circle></head-page-circle>
    </div>
    <div class="package">
      <molecule-card></molecule-card>
    </div>
    <div>
      <molecule-icon></molecule-icon>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import HeadPageCircle from "./components/organisms/HeadPageCircle.vue";
import MoleculeCard from "./components/molecules/MoleculeCard.vue";
import MoleculeIcon from "./components/molecules/MoleculeIcon.vue";

export default {
  name: "App",
  components: {
    HeadPageCircle,
    MoleculeCard,
    MoleculeIcon
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit:wght@300;400&display=swap');
* {
    margin: 0 !important;
    font-family: 'Kanit', sans-serif;
}
@media only screen and (max-width: 299px) {
  .head {
    margin-bottom: 680px !important;
  }
}
@media only screen and (min-width: 300px) and (max-width: 550px) {
  .head {
    margin-bottom: 640px !important;
  }
}
@media only screen and (min-width: 551px) and (max-width: 950px) {
  .head {
    margin-bottom: 350px !important;
  }
}
.package {
  margin-top: 30% !important;
  margin-bottom: 7% !important;
}
</style>
