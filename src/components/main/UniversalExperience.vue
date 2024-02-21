<script>
    export default{
        name: "UniversalExperience.vue",
        data(){
            return{
                TheBestTableInTown:[
                    {
                        titolo: 'the best table in town',
                        paragrafo: 'Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.',
                        // immag: '../assets/img/sushi-1.png',
                        bottone: 'explore the menu'
                    },
                ],
                PerfectForGroups:[
                    {
                        titolo: 'perfect for groups',
                        paragrafo: 'Quam eu proin sit massa condimentum. Volutpat non pulvinar aliquet nune. Orci elementum in aliquet a gravida vivamus aliquam turpis vitae.',
                        // immag: '../assets/img/sushi-1.png',
                        bottone: 'make a reservation'
                    },
                ],
                freshProduceEveryday:[
                    {
                        titolo: 'fresh produce everyday',
                        paragrafo: 'Hendrerit amet, volutpat leo non, commodo maecenas scelerisque tincidunt. Morbi vulputate morbi parus quisque sit sagittis orci alementum gravida.',
                        // immag: '../assets/img/sushi-1.png',
                        bottone: 'learn more about us'
                    },
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="d-flex justify-content-between mt-4">
        <div class="universalExperience">

            <div class="info mx-auto">

                <div>
                    <p><strong class="text-uppercase">hac tellus, felis risus at</strong> mattis mattis. Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi fauceibus elementum feugiat in nam in feugiat. Ipsum odio etiam duis facilisis amet vulpuatate.</p>
                    <h2>food is our common ground, a universal experience.</h2>
                    <br>
                    <p>Tristique tempus condimentum diam donee. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
                    <br>
                    <img src="../../assets/img/signature.jpg" width="130"  alt="">
                </div>
            </div>
            
        </div>

        <div class="imgSushi">
            <figure class="imgCaliforniaRolls">
                <!-- <img src="../../assets/img/info22x.jpg" alt=""> -->
                <div>
                    <h5>california rolls - $22</h5>
                </div>
            </figure>
        </div>
    </header>

    <main>
        <div class="p-5 d-flex justify-content-center">
            <div class="row text-center">
                
                <div class="col-4">
                    <!-- the best table in town -->
                    <div class="sezione">
                        <figure>
                            <img src="../../assets/img/sushi-1.png" alt="">
                        </figure>
                        <h4>{{ TheBestTableInTown[0].titolo }}</h4>
                        <p class="mt-4">{{ TheBestTableInTown[0].paragrafo }}</p>
                        <button class="button-white">{{ TheBestTableInTown[0].bottone }}</button>
                    </div>
                </div>

                <div class="col-4">
                    <!-- perfect for groups -->
                    <div class="sezione">
                        <figure>
                            <img src="../../assets/img/sushi-2.png" alt="">
                        </figure>
                        <h4>{{ PerfectForGroups[0].titolo }}</h4>
                        <p class="mt-4">{{ PerfectForGroups[0].paragrafo }}</p>
                        <button class="button-white">{{ PerfectForGroups[0].bottone }}</button>
                    </div>
                </div>

                <div class="col-4">
                    <!-- fresh produce everyday -->
                    <div class="sezione">
                        <figure>
                            <img src="../../assets/img/sushi-3.png" alt="">
                        </figure>
                        <h4>{{ freshProduceEveryday[0].titolo }}</h4>
                        <p class="mt-4">{{ freshProduceEveryday[0].paragrafo }}</p>
                        <button class="button-white">{{ freshProduceEveryday[0].bottone }}</button>
                    </div>
                </div>
            </div>
        </div>


        <div class="TheBestTableInTown d-flex justify-content-between mt-4">

            <div class="imgBestInTown">
            <!-- <img src="../../assets/img/slider32x.jpg" alt=""> -->
            </div>

            <div class="textBestInTown">
                <div class="fineDining mx-auto text-light">

                    <div class="d-flex align-items-center">
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
        </div>
    </main>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{

    .universalExperience{
        width: 50%;
        height: 90vh;

        .info{
            width: 500px;
            padding: 20px;
            margin-top: 80px;
        }
    }

    .imgSushi{
        width: 50%;
        height: 90vh;
        margin: 0;

        .imgCaliforniaRolls{
            position: relative;
            background-image: linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.6) 100%), url('../../assets/img/info22x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 440px;
            height: 575px;
            margin: 0 auto;
            margin-top: 50px;
            transition: all 0.5s ease 0s;

            &:hover{ // imgCaliforniaRolls
                transition: all 0.5s ease 0s;
                width: 460px; 
                height: 595px;
            }

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
}

main{

    .sezione{
        width: 325px;
    }

    .TheBestTableInTown{

        .textBestInTown{
            background-color: black;
            width: 35%;
            height: 75vh;

            .fineDining{
                width: 400px;
                margin-top: 110px;

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
    }
}
</style>

