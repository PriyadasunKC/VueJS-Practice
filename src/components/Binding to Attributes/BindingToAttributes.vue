<script setup>
</script>

<template>
    <div v-bind:id = "headingId">
        <h1>Binding to Attributes</h1>
        <p>Using v-bind to bind the value of id attribute</p>
        <input type="text" v-bind:disabled="isDisabled">
    </div>
</template>


<script>
export default {
  name: "BindingToAttributes",
  data() {
    return {
        headingId : "header",
        isDisabled : true
    };
  },
};
</script>

<style scoped>
    #header {
        text-align: center;
        color: blue;
    }
</style>




