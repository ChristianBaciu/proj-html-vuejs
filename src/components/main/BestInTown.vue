<script>
    export default{
        name: "BestInTown.vue",
        data(){

        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="d-flex justify-content-between">

        <div class="imgBestInTown">
        <!-- <img src="../../assets/img/slider32x.jpg" alt=""> -->
        </div>

        <div class="textBestInTown">
            <div class="bestTable mx-auto text-light">



                <div class="separatore d-flex align-items-center">
                    <div class="barra"></div>
                    <h5>fine dining experience</h5>
                </div>    



                <div class="info">
                    <h2>the best table in town</h2>
                    <br>
                    <p>Pellentesque vitae viverra risus. Venenatis ridiculus scelerisque nisi in urna nulla.</p>
                    <br>
                    <button class="button-black">explore the menu</button>
                </div>
            </div>
        </div>

    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    header{

        .textBestInTown{
            background-color: black;
            width: 35%;
            height: 75vh;

            .bestTable{
                width: 400px;
                margin-top: 125px;

                .info{
                    padding-top: 35px;
                    margin-left: 10px;
                    padding-left: 47px;
                }

                h5{
                    margin: 0;
                    margin-left: 20px;
                }
            }
        }

        .imgBestInTown{
            background-image: url('../../assets/img/slider32x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 65%;
            height: 75vh;
            margin: 0;
        }

        .titleLogo{
            padding: 20px;
        }
    }
</style>

