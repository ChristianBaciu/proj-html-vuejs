<script>
    export default{
        name: "AppMain.vue",
        data(){
            return{
                TheBestTableInTown:[
                    {
                        titolo: 'the best table in town',
                        paragrafo: 'Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.',
                        immag: '',
                        bottone: 'explore the menu'
                    },
                ],

                PerfectForGroups:[
                    {
                        titolo: 'perfect for groups',
                        paragrafo: 'Quam eu proin sit massa condimentum. Volutpat non pulvinar aliquet nune. Orci elementum in aliquet a gravida vivamus aliquam turpis vitae.',
                        immag: '',
                        bottone: 'make a reservation'
                    },
                ],

                freshProduceEveryday:[
                    {
                        titolo: 'fresh produce everyday',
                        paragrafo: 'Hendrerit amet, volutpat leo non, commodo maecenas scelerisque tincidunt. Morbi vulputate morbi parus quisque sit sagittis orci alementum gravida.',
                        immag: '',
                        bottone: 'learn more about us'
                    },
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="d-flex justify-content-between">
        <div class="experienceHeader">

            <div class="testo mx-auto">

                <div>

                    <p><strong>hac tellus, felis risus at</strong> mattis mattis. Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi fauceibus elementum feugiat in nam in feugiat. Ipsum odio etiam duis facilisis amet vulpuatate.</p>

                    <h2 class="text-uppercase">food is our common ground, a universal experience.</h2>
                    <br>
                    <p>Tristique tempus condimentum diam donee. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
                    <br>
                    <img src="../assets/img/signature.jpg" width="110"  alt="">
                </div>
            </div>
            
        </div>

        <div class="imgHeader">

            <img src="../assets/img/info22x.jpg" width="400" alt="">

        </div>


    </header>

    <main>
        <div class="informazione p-5 d-flex justify-content-center">
            <div class="row">
                <div class="col-4">
                    <div class="sezione">

                        <img src="" alt="">

                        <h3>{{ TheBestTableInTown[0].titolo }}</h3>
                        <p>{{ TheBestTableInTown[0].paragrafo }}</p>
                        <button>{{ TheBestTableInTown[0].bottone }}</button>
                    </div>
                </div>

                <div class="col-4">
                    <div class="sezione">

                        <img src="" alt="">

                        <h3>{{ PerfectForGroups[0].titolo }}</h3>
                        <p>{{ PerfectForGroups[0].paragrafo }}</p>
                        <button>{{ PerfectForGroups[0].bottone }}</button>
                    </div>
                </div>

                <div class="col-4">
                    <div class="sezione">

                        <img src="" alt="">

                        <h3>{{ freshProduceEveryday[0].titolo }}</h3>
                        <p>{{ freshProduceEveryday[0].paragrafo }}</p>
                        <button>{{ freshProduceEveryday[0].bottone }}</button>
                    </div>
                </div>  
            </div>
        </div>
    </main>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    ul{
        list-style-type: none;
    }

    header{

        .experienceHeader{
            width: 50%;
            // background-color: orange;
            height: 95vh;

            .testo{
                // background-color: blue;
                width: 500px;
                padding: 20px;
                margin-top: 100px;
            }

        }

        .imgHeader{
            // // background-color: red;
            width: 50%;
            height: 95vh;
            margin: 0;

            img{
                margin-top: 100px;
                margin-left: 25px;
            }
        }
    }

    main{
        background-color: orange;

        .informazione{
            
        }


        .sezione{
            width: 400px;
            background-color: blue;
        }
    }


</style>

