<template>
  <div class="row justify-content-center box-icon">
    <div class="col-1 mt-5">
      <img class="ant" src="@/assets/ant.png">
    </div>
    <div class="col-11">
      <div class="row justify-content-end mt-5">
        <atom-icon
          :title="'ราคาเบาๆ'"
          :text="'ความคุ้มครองครอบคลุมในราคาที่เหมาะสม'"
          :pic="'wallet.png'"
          class="col-lg-4 col-md-12 col-sm-12"
        ></atom-icon>
        <atom-icon
          :title="'ป่วยไม่กลัว'"
          :text="'ความคุ้มครองครอบคลุมในราคาที่เหมาะสม'"
          :pic="'hospital.png'"
          class="col-lg-4 col-md-12 col-sm-12"
        ></atom-icon>
      </div>
      <div class="row justify-content-end mt-3 mb-5">
        <atom-icon
          :title="'จัดเต็มทุกเส้นทาง'"
          :text="'มีบรกิารช่วยเหลือฉุกเฉิน พร้อมติดต่อได้ 24 ชั่วโมง'"
          :pic="'woman.png'"
          class="col-lg-4 col-md-12 col-sm-12"
        ></atom-icon>
        <atom-icon
          :title="'มั่นใจ Jaadhai'"
          :text="'รับประกันโดยบริษัท โอ เอส จี ประกันภัย'"
          :pic="'shield.png'"
          class="col-lg-4 col-md-12 col-sm-12"
        ></atom-icon>
      </div>
    </div>
  </div>
</template>

<script>
import AtomIcon from "../atoms/AtomIcon.vue";

export default {
  name: "MoleculeIcon",
  components: {
    AtomIcon,
  },
};
</script>

<style scoped>
@media only screen and (max-width: 299px) {
  .ant {
    display: none;
  }
}
@media only screen and (min-width: 300px) and (max-width: 550px) {
  .ant {
    display: none;
  }
}
@media only screen and (min-width: 551px) and (max-width: 950px) {
  .ant {
    display: none;
  }
}  
.box-icon {
  background-color: #FFFAE6;
}
.ant {
  margin-left: 150px !important;
}
</style>
