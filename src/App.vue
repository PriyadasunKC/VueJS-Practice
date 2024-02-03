<script setup>
import HelloWorld from "./components/dynamicTexts/HelloWorld.vue";
import BindingToAttributes from "./components/Binding to Attributes/BindingToAttributes.vue";
</script>

<template>
  <div class="firstDiv">{{ greet }} {{ name }}</div>
  <div v-text="channel"></div>
  <HelloWorld />
  <BindingToAttributes />
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
