<template>
    <div class="modal">
        <div class="overlay" @click ="$emit('close-modal')"></div>
        <div class="modal-card">
            <slot />
        </div>
    </div>
</template>

<script>
export default{};
</script>

<style>
.modal{
    margin-top:100px;
}
.overlay{
    width:100%;
    height:100%;
    position: fixed;
    left:0;
    top: 0;
}
.overlay{
    opacity: 0.5;
    background-color:black;
}
.modal-card{
    position: relative;
    max-width: 90%;
    margin: auto;
    margin-top:20px;
    padding:20px;
    background-color: white;
    min-height: 500px;
    z-index: 10;
    opacity:1;
}
</style>