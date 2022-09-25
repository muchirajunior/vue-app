<template>
  <h1> {{title}} </h1>
  <h4>{{name}}</h4>
  <span>{{location}}</span>
  <MyModal header="The About Us Modal" />
</template>

<script>
  import MyModal from "./components/Modal.vue"

  export default {
    name: 'App',
    components:{ MyModal},
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
    background-color: #bbbcbd;
    min-height: 90vh;
  }
</style>