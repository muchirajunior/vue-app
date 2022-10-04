<template>
    <div class="container">
        <span class="head">The Ninja Timer </span>
        <button class="btn-play" @click="tongleTimer()"  :disabled="play">play </button>
        <Block v-if="play"/>
        <Results  />
    </div>
</template>

<script >
import Block from './Block.vue';
import Results from './Results.vue';
    export default{
    data() {
        return {
            play: false,
            delay:2000,
            results:0
        };
    },
    methods: {
        tongleTimer() {
            this.play = !this.play;
            console.log(this.play ? "start timer" : "stop timer");
        }
    },
    components: { Block, Results }
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