<template>
  <div>
    <input
      :type="type"
      :placeholder="placeholder"
      :value="value"
      :size="size"
      class="p-2"
      :class="sizeButton"
    />
  </div>
</template>

<script>
export default {
  name: "AtomInput",
  props: {
    type: {
      type: String,
      require: true,
    },
    placeholder: {
      type: String,
      require: false,
    },
    value: {
      type: String,
      require: false,
    },
    size: {
      type: String,
      require: false,
    },
  },
  computed: {
    sizeButton() {
      if (this.size === "sm") return "bt--small";
      else if (this.size === "lg") return "bt--lg";
      else return "";
    },
  }
};
</script>

<style scoped>
input[type="text"] {
  width: 100%;
  border: 1px solid rgb(192, 192, 192);
  border-radius: 10px;
}  
input[type="date"] {
  width: 100%;
  border: 1px solid rgb(192, 192, 192);
  border-radius: 10px;
}
.bt--lg {
  color: white;
  width: 100%;
  border: none;
  border-radius: 20px;
  background-color: #C60000;
}
.bt--small {
  color: white;
  width: 50%;
  border: none;
  border-radius: 20px;
  background-color: #C60000;
}
</style>
