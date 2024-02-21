<script>
    export default{
        name: "Menu.vue",
        data(){
            return{
                
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
