
<template>
    <!-- adding static classes -->
    <h2 class="text_success">Success Text</h2>
    <!-- adding dynamic classes -->
    <h2 class="text_success" v-bind:class="status">Status</h2>

    <!-- adding  multiple classes -->
    <h2 v-bind:class="[status, 'text_success']">Multiple Classes</h2>

    <!-- adding  classes with condition -->
    <h2 v-bind:class="isPromoted ?'promoted':'text_success'">Promoted</h2>

    <!-- adding  classes arrays with condition -->
    <h2 v-bind:class="[isPromoted && 'promoted', isSold ? 'danger' : 'isSold']">Arrays with condition</h2>

    <!-- adding  classes objects with condition -->
    <h2 v-bind:class="{
        promoted: isPromoted,
        isSold: isSold,
        'sold': status,
    }"> Object Conditional approach apply classes</h2>
</template>

<script>
export default {
  name: "BindingClasses",
  data() {
    return {
        status : 'danger',
        isPromoted: true,
        isSold: false
    };
  },
};
</script>

<style scoped>
    .text_success {
        text-decoration: underline;
        text-align: center;
    }

    .danger {
        color: red;
        text-align: center;
    }

    .promoted {
        color:coral;
        font-style: italic;
        text-align: center;
    }

    .isSold {
        color: green;
        font-size: 2rem;
        text-align: center;
    }


</style>
