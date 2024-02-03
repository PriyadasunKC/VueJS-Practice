<script setup>
import HelloWorld from "./components/dynamicTexts/HelloWorld.vue";
</script>

<template>
  <div class="firstDiv">{{ greet }} {{ name }}</div>
  <div v-text="channel"></div>
  <HelloWorld />
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Chathura",
      greet: "Hello",
      channel: "CodEvo",
    };
  },
};
</script>

<style scoped>
.firstDiv {
  color: red;
  text-align: center;
}
</style>
