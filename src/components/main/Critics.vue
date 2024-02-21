<script>
    export default{
        name: "Critics.vue",
        data(){
            return{
                NewYorkTimes:[
                    {
                        titolo: 'new york times',
                        paragrafo: 'Non arcu mauris tortor ultrices molis tellus euismod fermentum. Habitant amet tincidunt id sapien accumsan sed at',
                        SecondoParagrafo: 'Mmalesauda ullamcorper amet. Pretium pretium dignissim nisi.',
                        bottone: 'read full article'
                    },
                ],
                TheGuardian:[
                    {
                        titolo: 'the guardian',
                        paragrafo: 'Non arcu mauris tortor ultrices molis tellus euismod fermentum. Habitant amet tincidunt id sapien accumsan sed.',
                        bottone: 'read full article'
                    },
                ],
                GlobeAndMail:[
                    {
                        titolo: 'globe and mail',
                        paragrafo: 'Vivamus magna justo, lacinia eget conseetetur sed, convallis at tellus. Nulla porttitor accumsan tincidunt.',
                        bottone: 'read full article'
                    },
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="d-flex flex-column align-items-center">
        <p class="titleCritics p-5">What critics are saying about us</p>



        <div class="critiche">
            <div class="NewYorkTimes d-flex justify-content-between">
                <figure>
                    <img src="../../assets/img/blog72x.jpg" alt="">
                </figure>

                <div class="info text-light mx-auto">
                    <h5>fine dining experience</h5>
                    <h2>{{ NewYorkTimes[0].titolo }}</h2>

                    <span v-for="(stelle, index) in 5" :key="index">
                        <i class="fas fa-star"></i>
                    </span>

                    <div class="barra my-4"></div>

                    <p>{{ NewYorkTimes[0].paragrafo }}</p>
                    <p class="mb-5">{{ NewYorkTimes[0].SecondoParagrafo }}</p>
                    <button class="button-black">{{ NewYorkTimes[0].bottone }}</button>
                </div>
            </div>

            <div class="d-flex justify-content-between">
                <div class="GlobeAndMail">
                    <!-- <img src="../../assets/img/info52x.jpg" alt=""> -->
                    <div class="info text-light mx-auto">
                        <h5>fine dining experience</h5>
                        <h2>{{ TheGuardian[0].titolo }}</h2>

                        <span v-for="(stelle, index) in 5" :key="index">
                            <i class="fas fa-star"></i>
                        </span>

                        <div class="barra my-4"></div>

                        <p class="mb-5">{{ TheGuardian[0].paragrafo }}</p>
                        <button class="button-hybrid">{{ TheGuardian[0].bottone }}</button>
                    </div>
                </div>

                <div class="TheGuardian bg-danger">
                    <!-- <img src="../../assets/img/info12x.jpg" alt=""> -->
                    <div class="info text-light mx-auto">
                        <h5>fine dining experience</h5>
                        <h2>{{ GlobeAndMail[0].titolo }}</h2>

                        <span v-for="(stelle, index) in 5" :key="index">
                            <i class="fas fa-star"></i>
                        </span>

                        <div class="barra my-4"></div>

                        <p class="mb-5">{{ GlobeAndMail[0].paragrafo }}</p>
                        <button class="button-hybrid">{{ GlobeAndMail[0].bottone }}</button>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <main>

        <figure class="imgKunPaoChicken my-5">
            <!-- <img src="../../assets/img/page52x.jpg" alt=""> -->
            <div>
                <h5>kung pao chicken - $32</h5>
            </div>
        </figure>

    </main>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{
    .titleCritics{
      font-size: 30px;
    }

    .critiche{

        .NewYorkTimes{
            background-color: black;
            width: 1000px;
            margin-bottom: 40px;

            figure{
                margin: 0px;

                img{
                    width: 500px;
                    height: 570px;
                }
            }

            .info{
                width: 350px;
                margin-top: 100px;
            }
        }

        .GlobeAndMail, .TheGuardian{
            width: calc(50% - 20px);
            height: 480px;
        }

        .GlobeAndMail{
            background-image: linear-gradient(0deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.9) 100%), url('../../assets/img/info52x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;

            .info{
                width: 350px;
                margin-top: 60px;
            }

        }

        .TheGuardian{
            background-image: linear-gradient(0deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.9) 100%), url('../../assets/img/info12x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;

            .info{
                width: 350px;
                margin-top: 80px;
            }
        }
    }
}

main{

    .imgKunPaoChicken{
        position: relative;
        background-image: linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.7) 100%), url('../../assets/img/page52x.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 500px;

        div{
            position: absolute;
            bottom: 5px;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            color: white;
        }
    }
}
</style>
