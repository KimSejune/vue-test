<template>
  <div>
    <h1>Hello {{ value }}</h1>
    <button name="my-btn" @click="changeProp()"></button>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: "Test",
    },
  },
  method: {
    changeProp() {
      this.value = "change";
    },
  },
};
</script>
