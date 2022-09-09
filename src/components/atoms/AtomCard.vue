<template>
  <div class="card m-2 p-0">
    <img class="card-img-top" :src="require(`@/assets/${pic}`)" />
    <div class="card-body mt-2">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ text }}</p>
      <atom-input
        :type="'submit'"
        :value="'เลือกแพ็กเกจนี้'"
        :size="'sm'"
        class="mt-5 d-flex justify-content-end"
      ></atom-input>
    </div>
  </div>
</template>

<script>
import AtomInput from "./AtomInput.vue";

export default {
  name: "AtomCard",
  props: {
    title: {
      type: String,
      require: true,
    },
    text: {
      type: String,
      require: true,
    },
    pic: {
      type: String,
      require: true,
    },
  },
  components: {
    AtomInput,
  },
};
</script>

<style>
.card {
  width: 300px !important;
  border: none !important;
  border-radius: 12px !important;
  box-shadow: 2px 2px rgba(228, 228, 228, 0.3);
}
</style>
