<template>
  <h1> {{title}} </h1>
  <h4>{{name}}</h4>
</template>

<script>

  export default {
    name: 'App',
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
    margin-top: 60px;
  }
</style>