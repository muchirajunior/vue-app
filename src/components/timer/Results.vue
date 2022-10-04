<template>
    <div class="result">
        <h5>Timer results :</h5>
        <p>{{results}} seconds</p>
    </div>
</template>

<script>
    export default{
        name:"TimerResults",
        props:["results"],

    }
</script>

<style scoped> 
    .result{
        display: block;
        text-align: center;
    }
    p{
        color: aqua;
    }
</style>