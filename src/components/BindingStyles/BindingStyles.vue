<template>
  <h2
    v-bind:style="{
      color: backColor,
      fontSize: headerSize + 'px',
    }"
  >
    Style by js Object
  </h2>
  <h2 :style="styleObject">Style by js Object</h2>

  <!--apply multiple Styles using array -->
  <h2 v-bind:style="[styleObject1,styleObject2]"> Styles using array</h2>
</template>

<script>
export default {
  name: "BindingStyles",
  data() {
    return {
      backColor: "burlywood",
      headerSize: "50",

      styleObject: {
        color: "red",
        fontSize: "50px",
        fontFamily: "Arial",
      },

      styleObject1: {
        fontSize: "50px",
        fontFamily: "Arial",
      },

      styleObject2: {
        color: "blue",
        border: "2px solid black",
      },
    };
  },
};
</script>

<style scoped>
</style>
