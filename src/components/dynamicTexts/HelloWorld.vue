<script setup>
import dyStyles from "./dynmicStyles.module.css";
</script>

<template>
    <div v-html="msg" :class="dyStyles.hw"></div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "<b>Hello World</b>",
    };
  },
};
</script>

<style scoped>

</style>
