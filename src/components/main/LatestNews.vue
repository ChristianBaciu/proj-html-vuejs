<script>
    export default{
        name: "LatestNews.vue",
        data(){

        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    
    <div class="text-center">
        <p style="font-size: 30px;">Latest news E promotions</p>
    </div>

    <div class="promotions mx-auto bg-primary">
        <div class="d-flex">  <!-- justify-content-between -->

            <div class="clo-4 bg-danger">
                <figure>
                    <!-- <img src="../../assets/img/blog92x.jpg" alt=""> -->
                </figure>
                <h1>ciao</h1>
            </div>
            <div class="clo-4 bg-warning">
                <figure>
                    <!-- <img src="../../assets/img/blog72x.jpg" alt=""> -->
                </figure>
                <h1>ciao</h1>
            </div>
            <div class="clo-4 bg-secondary">
                <figure>
                    <!-- <img src="../../assets/img/blog82x.jpg" alt=""> -->
                </figure>
                <h1>ciao</h1>
            </div>

        </div>
    </div>









    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>

    <div class="TheBestTableInTown d-flex justify-content-between">

        <figure class="imgBestInTown">
        <!-- <img src="../../assets/img/slider32x.jpg" alt=""> -->
        </figure>

        <div class="textBestInTown">
            <div class="enjoyYour mx-auto text-light">

                <div class="d-flex align-items-center">
                    <div class="barra"></div>
                    <h5>enjoy your meal at home</h5>
                </div>    

                <div class="info">
                    <h2>takeout now available</h2>
                    <br>
                    <p>Pellentesque vitae viverra risus, sagittis Venenatis ridiculus scelerisque nisi in urna nulla non arcu moris tortor.</p>
                    <br>
                    <button class="button-black"><i class="fa-solid fa-car me-2"></i>explore the menu</button>
                </div>
            </div>
        </div>
    </div>

    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>
    <br><br>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

.promotions{
    width: 1000px;
}





.TheBestTableInTown{

    .textBestInTown{
        background-color: black;
        width: 35%;
        height: 80vh;

        .enjoyYour{
            width: 400px;
            margin-top: 120px;

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
        background-image: url('../../assets/img/slider72x-scaled.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        width: 65%;
        height: 80vh;
        margin: 0;
    }
}

</style>

