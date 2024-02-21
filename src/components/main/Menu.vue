<script>
    export default{
        name: "Menu.vue",
        data(){
            return{
                horsDOeuvres:[
                    {
                        menu: "hors d'oeuvre",
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
            <div class="horsDOeuvres bg-primary">
                <div class="info text-light mx-auto p-5">

                    <h3>{{ horsDOeuvres[0].menu }}</h3>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p class="bg-danger">descrizione piatto</p>

                    <!-- <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>


                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p> -->

                </div>
            </div>

            <div class="mainCourse bg-warning">
                <!-- <img src="../../assets/img/misc22x.jpg" alt=""> -->
                <div class="info text-light mx-auto  p-5">

                    <h3>menu</h3>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>

                    <!-- <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>


                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p> -->

                </div>
            </div>

            <div class="dessert bg-secondary">

                <div class="info text-light mx-auto p-5">

                    <h3>menu</h3>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>

                    <!-- <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>

                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p>


                    <div class="d-flex justify-content-between bg-danger my-3">
                        <h4>nomepiatto</h4>
                        <div>prezzo</div>
                    </div>
                    <p>descrizione piatto</p> -->

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
        }
    
        .mainCourse{
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
