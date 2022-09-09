<template>
  <div class="box-input p-3">
    <h2 class="text-center mt-3 mb-5">จัดให้จัดเต็มทุกการเดินทาง</h2>
    <div class="row justify-content-start mt-3">
      <atom-input
        class="col-lg-6 col-md-12 col-sm-12 mb-3"
        :type="'text'"
        :placeholder="'ต้นทาง'"
      ></atom-input>
      <atom-input
        class="col-lg-6 col-md-12 col-sm-12 mb-3"
        :type="'text'"
        :placeholder="'ปลายทาง'"
      ></atom-input>
    </div>
    <div class="row justify-content-start">
      <atom-input
        class="col-lg-6 col-md-12 col-sm-12 mb-3"
        :type="'text'"
        :placeholder="'วันที่ไป'"
      ></atom-input>
      <atom-input
        class="col-lg-6 col-md-12 col-sm-12 mb-3"
        :type="'text'"
        :placeholder="'วันที่กลับ'"
      ></atom-input>
    </div>
    <div class="row justify-content-cecnter">
      <atom-form :text="'ประเภทการเดินทาง'" class=""></atom-form>
      <atom-form :text="'จำนวนผู้เดินทาง'" class="mt-3"></atom-form>
    </div>
    <atom-input :type="'submit'" :value="'เช็คราคา'" :size="'lg'" class="mt-5"></atom-input>
    <div class="text-footer text-center row justify-content-center mt-3">
      <p class="col-lg-4">ขั้นตอนการซื้อ</p>
      <p class="col-lg-4">ข้อมูลผลิตภัณฑ์</p>
    </div>
  </div>
</template>

<script>
import AtomInput from "../atoms/AtomInput.vue";
import AtomForm from "../atoms/AtomForm.vue";

export default {
  name: "MoleculeInput",
  components: {
    AtomInput,
    AtomForm,
  },
};
</script>

<style scoped>
.box-input {
  background-color: rgb(255, 255, 255);
  border: none;
  border-radius: 12px;
}
.text-footer {
  color: rgb(107, 175, 103);
  text-decoration: underline;
}
</style>
