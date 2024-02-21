<script>
    export default{
        name: "Menu.vue",
        data(){
            return{
                horsDOeuvres:[
                    {
                        menu: "hors d'oeuvres",
                        piatti:[
                            {
                                nomeDelPiatto: 'ahi salmon nigiri',
                                descrizione: 'Eget vulputate vitate quis retrum blandit sed. quam nulla sit lacinia.',
                                prezzo: '$48'
                            },
                            {
                                nomeDelPiatto: 'umi masu salad',
                                descrizione: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                                prezzo: '$21'
                            },
                            {
                                nomeDelPiatto: 'temak wih crab',
                                descrizione: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
                                prezzo: '$32'
                            },
                            {
                                nomeDelPiatto: 'california rolls',
                                descrizione: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
                                prezzo: '$22'
                            }
                        ]
                    }
                ],

                mainCourse:[
                    {
                        menu: 'main course',
                        piatti:[
                            {
                                nomeDelPiatto: 'braised abalone',
                                descrizione: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                                prezzo: '$52'
                            },
                            {
                                nomeDelPiatto: 'twice cooked pork',
                                descrizione: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
                                prezzo: '$21'
                            },
                            {
                                nomeDelPiatto: 'temak wih crab',
                                descrizione: 'Quis duis sit dictum aliquem a velit enim. Tellus in sit augue aliquam.',
                                prezzo: '$32'
                            },
                            {
                                nomeDelPiatto: 'california rolls',
                                descrizione: 'Feugiat rhoncus ipsum tristique purus diam, et dolor molestie.',
                                prezzo: '$48'
                            }
                        ]
                    }
                ],

                dessert:[
                    {
                        menu: 'dessert',
                        piatti:[
                            {
                                nomeDelPiatto: 'choccolate ball cake',
                                descrizione: 'In pellentesque in felis massa vehicula. In sed euismod ut',
                                prezzo: '$13'
                            },
                            {
                                nomeDelPiatto: 'lime pie with crust',
                                descrizione: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                                prezzo: '$14'
                            },
                            {
                                nomeDelPiatto: 'rasberry pear cake',
                                descrizione: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit.',
                                prezzo: '$18'
                            },
                            {
                                nomeDelPiatto: 'café au lait',
                                descrizione: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit.',
                                prezzo: '$6'
                            }
                        ]
                    }
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="my-5 py-5">
        <div class="menu d-flex justify-content-center">
            
            <div class="horsDOeuvres">
                <h3 class="p-5">{{ horsDOeuvres[0].menu }}</h3><!-- nome menu -->

                <div v-for="(element, index) in horsDOeuvres[0].piatti" :key="index"
                class="info text-light mx-auto pb-4 px-5">

                    <div class="d-flex justify-content-between text-dark">
                        <h4>{{ element.nomeDelPiatto }}</h4>
                        <div>{{ element.prezzo }}</div>
                    </div>
                    <p class="text-dark">{{ element.descrizione }}</p>
                </div>
            </div>

            <div class="mainCourse">
                <h3 class="p-5 text-light">{{ mainCourse[0].menu }}</h3><!-- nome menu -->

                <div v-for="(element, index) in mainCourse[0].piatti" :key="index"
                class="info text-light mx-auto pb-4 px-5">

                    <div class="d-flex justify-content-between text-light">
                        <h4>{{ element.nomeDelPiatto }}</h4>
                        <div>{{ element.prezzo }}</div>
                    </div>
                    <p>{{ element.descrizione }}</p>
                </div>
            </div>

            <div class="dessert">
                <h3 class="p-5">{{ dessert[0].menu }}</h3><!-- nome menu -->

                <div v-for="(element, index) in dessert[0].piatti" :key="index"
                class="info text-light mx-auto pb-4 px-5">

                    <div class="d-flex justify-content-between text-dark">
                        <h4>{{ element.nomeDelPiatto }}</h4>
                        <div>{{ element.prezzo }}</div>
                    </div>
                    <p class="text-dark">{{ element.descrizione }}</p>
                </div>
            </div>

        </div>
    </header>


    <main>
        <figure>
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
    </main>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{
    
    .menu{
        
        .horsDOeuvres, .mainCourse, .dessert{
            width: 450px;
            background-color: #e8e8e8;
        }
    
        .mainCourse{
            background-image: linear-gradient(0deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.9) 100%), url('../../assets/img/misc22x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            margin-top: -30px;
            margin-bottom: 30px;
        }
    }
}

main{

    figure{
        position: relative;
        background-image: url('../../assets/img/hero42x.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 650px;
        margin: 0px;
    }

    .BraisedAbalone{
        position: absolute;
        background-color: black;
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
