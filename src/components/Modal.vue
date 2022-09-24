<template>
    <div class="backdrop">
        <div class="modal">
            <div class="modal-content">
                modal content
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        name:"MyModal"
    }
</script>

<style>
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
        background: rgb(134, 130, 130);
    }
</style>