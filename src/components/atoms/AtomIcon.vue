<template>
  <div class="row justify-content-start">
    <img class="col-6" :src="require(`@/assets/${pic}`)" />
    <div class="col-6 align-self-center">
      <h5>{{ title }}</h5>
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "AtomIcon",
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
};
</script>

<style scoped>
img {
  width: 120px !important;
}
p {
  font-size: 13px;
}
</style>
