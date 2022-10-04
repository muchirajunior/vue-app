<template>
  <!-- <MyModal header="The About Us Modal" text="Grab our new offers from the new outlets, yeeeeey !!!" /> -->
  <!-- <NinjaTimer /> -->
  <MyForm />
</template>

<script>

import MyForm from "./components/forms/form.vue";

  export default {
    name: 'App',
    components:{ MyForm},
    data() {
      return {
        title: "Hello world Vue (:",
        name: "muchira junior",
        location:"This Location"
      }
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    background-color: rgb(226, 225, 225);
    min-height: 100vh;
    padding-top: 30px;
    margin: 0;
  }
</style>