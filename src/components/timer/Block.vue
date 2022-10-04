<template>
    <div class="block"  v-f="showBlock">
        click me 
    </div>
</template>


<script>

    export default{
        name:"TimerBlock",
        props:["delay"],
        data(){
            return{
                showBlock:false
            }
        },
        methods:{
            mounted(){
                console.log("block component mounted");
                setTimeout(() => {
                    this.showBlock=true;
                }, this.delay);
            },

            updated(){
                console.log("block compone")
            }
        }
    }
</script>

<style>
    .block{
        width: 400px;
        padding: 100px;
        text-align: center;
        margin: 100px auto;
        background: rgb(1, 82, 1);
        color: white;
        border-radius: 20px;
    }

</style>