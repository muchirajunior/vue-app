<template>
  <!-- <MyModal header="The About Us Modal" text="Grab our new offers from the new outlets, yeeeeey !!!" /> -->
  <NinjaTimer />
</template>

<script>

import NinjaTimer from "./components/NinjaTimer.vue";

  export default {
    name: 'App',
    components:{  NinjaTimer },
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
    padding-top: 60px;
    background-color: white;
    min-height: 90vh;
  }
</style>