<script>
    export default{
        name: "ButtonOptions.vue",
        data(){

        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header>
        <div class="options d-flex flex-column justify-content-center align-items-center">
            <i class="fa-solid fa-cart-shopping  d-flex justify-content-center align-items-center"></i>
            <h6>Prebuilts</h6>
        </div>

        <div class="options d-flex flex-column justify-content-center align-items-center" style="top: 43%;">
            <i class="fa-solid fa-folder  d-flex justify-content-center align-items-center"></i>
            <h6>Prebuilts</h6>
        </div>
    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

.options{
    background-color: white;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
    border-radius: 5px;
    position: fixed;
    z-index: 999;
    top: 30%;
    right: 0%;
    margin-right: 20px;
    padding: 17px;
    cursor: pointer;

    h6{
        margin: 0;
    }
    
    i{
        width: 40px;
        height: 40px;
    }
}
</style>