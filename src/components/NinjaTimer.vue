<template>
    <div class="container">
        <span class="head">The Ninja Timer</span>
        <button class="btn-play" @click="tongleTimer()">{{play ? "Play":"Pause"}}</button>
    </div>
</template>

<script >
    export default{
        data(){
            return {
                play:true
            }
        },
        methods:{
            tongleTimer(){
                this.play=!this.play;
                console.log(this.play ? "start timer":"stop timer");
            }

        }
    }
</script>

<style scoped>
    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .head{
        color: aqua;
        font-weight: bold;
        font-size: 20px;
        margin: 20px;
    }
    .btn-play{
        background-color:  aqua;
        border: none;
        outline: none;
        padding: 10px;
        width: 200px;
        margin: auto;
        border-radius: 10px;
        font-weight: bold;

    }
</style>