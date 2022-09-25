<template>
    <div class="backdrop" @click="closeModal()">
        <div class="modal">
            <div class="modal-header"> {{header}} </div>
            <div class="modal-content">{{text}} </div>
        </div>
    </div>
</template>

<script>
    export default{
        name:"MyModal",
        props:["header","text"],
        methods:{
        closeModal(){
            this.$emit("close")
            console.log("closing modal;");
            let modal=document.getElementsByClassName("backdrop");
            modal.style.display ="none";   
        }
    }
    }
</script>

<style scoped>
    .modal{
        width: 400px;
        padding: 20px;
        margin: 100px auto;
        background: white;
        border-radius: 10px;
    }

    .backdrop{
        width: 100%;
        height: 100%;
        top: 0;
        position: fixed;
        background: rgba(0, 0, 0,.5);
    }
    .modal-header{
        color: rgb(17, 149, 182);
        font-size: 20px;
        font-weight: bold;
        margin-bottom: 20px;
        margin-top: 20px;
    }

</style>