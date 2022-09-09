<template>
  <div class="mt-5 mb-5">
    <h3 class="text-center mb-3">แพ็กเกจ</h3>
    <div class="row justify-content-center">
      <atom-card
      :title="'Overseas'"
      :text="'แพ็กเกจสำรับนักเดินทางต่างประเทศที่รักความคล่องตัวผจญภัยไปไหน ไม่ต้องกังวล'"
      :pic="'image 15.png'"
      class="col-lg-6 col-md-12 col-sm-12"
      ></atom-card>
      <atom-card
      :title="'Family'"
      :text="'แพ็กเกจสำรับนักเดินทางต่างประเทศที่รักความคล่องตัวผจญภัยไปไหน ไม่ต้องกังวล'"
      :pic="'image 15_2.png'"
      class="col-lg-6 col-md-12 col-sm-12"
      ></atom-card>
    </div>
  </div>
</template>

<script>
import AtomCard from "../atoms/AtomCard.vue";

export default {
  name: "MoleculeCard",
  components: {
    AtomCard,
  },
};
</script>

<style></style>
