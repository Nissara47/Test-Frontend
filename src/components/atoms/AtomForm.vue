<template>
  <div>
    <select class="p-2 w-100">
      <option selected disabled hidden>{{ text }}</option>
      <option>1</option>
      <option>2</option>
      <option>3</option>
    </select>
  </div>
</template>

<script>
export default {
  name: 'AtomForm',
  props: {
    text: {
      type: String,
      require: true,
    }      
  }
}
</script>

<style scoped>
select {
  border-radius: 10px;
  border: 1px solid rgb(192, 192, 192);
}
</style>