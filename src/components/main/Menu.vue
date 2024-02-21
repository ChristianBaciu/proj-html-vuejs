<script>
    export default{
        name: "Menu.vue",
        data(){

        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header>
        <figure class="imgKunPaoChicken">
            <!-- <img src="../../assets/img/hero42x.jpg" alt=""> -->
            <nav class="BraisedAbalone">

                <div class="info mx-auto text-light">
                    <div class="d-flex">

                        <h2>braised abalone</h2>
                        <h5 class="mt-2">$52</h5>
                    </div>

                    <div class="barra my-4"></div>

                    <p>Pretium accumsan porttitor viverra leo gravida mollis imperdiet. Fringilla nibh pharetra sociis leo amet.</p>
                    <button class="button-black my-4">view in the menu</button>
                </div>
            </nav>
        </figure>
    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{

    figure{
        position: relative;
        background-image: linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.7) 100%), url('../../assets/img/hero42x.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 650px;
        margin: 0px;
    }

    .BraisedAbalone{
        background-color: black;
        position: absolute;
        top: 50%;
        left: 20%;
        transform: translate(-50%, -50%);
        height: 500px;
        width: 450px;

        .info{
            width: 300px;
            margin-top: 90px;
        }
    }
}
</style>
