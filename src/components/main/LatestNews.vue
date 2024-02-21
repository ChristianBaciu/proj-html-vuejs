<script>
    export default{
        name: "LatestNews.vue",
        data(){

        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    
    <div class="text-center my-5">
        <p style="font-size: 30px;">Latest news &#8455; promotions</p>
    </div>

    <div class="promotions mx-auto">
        <div class="d-flex justify-content-center text-center gap-4">

            <div class="theBestCoffeInTown col-4">
                <figure>
                    <!-- <img src="../../assets/img/blog92x.jpg" alt=""> -->
                </figure>
                <h4>the best coffee in town</h4>
                <p>By admin<span class="mx-3">Published On: Jenuary 7th, 2020</span>Categories: News</p>
            </div>
            
            <div class="discoverOurNewMenu col-4">
                <figure>
                    <!-- <img src="../../assets/img/blog72x.jpg" alt=""> -->
                </figure>
                <h4>discover our new menu</h4>
                <p>By admin<span class="mx-3">Published On: Jenuary 7th, 2020</span>Categories: News</p>
            </div>

            <div class="weNowAcceptSquare col-4">
                <figure>
                    <!-- <img src="../../assets/img/blog82x.jpg" alt=""> -->
                </figure>
                <h4>we now accept square!</h4>
                <p>By admin<span class="mx-3">Published On: Jenuary 7th, 2020</span>Categories: News</p>
            </div>

        </div>
    </div>


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

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

.promotions{
    width: 1250px;

    h4{
        margin-top: 25px;
    }

    p{
        font-size: 12px;
    }

    .theBestCoffeInTown, .discoverOurNewMenu, .weNowAcceptSquare{
        figure{
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            height: 500px;
            margin: 0;
        }
    }

    .theBestCoffeInTown{
        figure{
            background-image: url('../../assets/img/blog92x.jpg');
        }
    }

    .discoverOurNewMenu{
        figure{
            background-image: url('../../assets/img/blog72x.jpg');
        }
    }

    .weNowAcceptSquare{
        figure{
            background-image: url('../../assets/img/blog82x.jpg');
        }
    }
}

.TheBestTableInTown{
    margin-top: 30px;

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

