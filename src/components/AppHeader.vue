<script>
    export default{
        name: "AppHeader.vue",
        data(){
            return{
                headerAvada:[
                    {
                        nome: 'Home',
                        // true
                    },
                    {
                        nome: 'Culinary History',
                        // false
                    },
                    {
                        nome: 'Our Team',
                        // false
                    },
                    {
                        nome: 'Our Menu',
                        // false
                    },
                    {
                        nome: 'Takeout',
                        // false
                    },
                    {
                        nome: 'Bulletin',
                        // false
                    },
                    {
                        nome: 'Reservations',
                        // false
                    },
                    {
                        // nome: '<i class="fa-solid fa-cart-shopping"></i>'
                        // false
                    }
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header class="d-flex justify-content-between">
        <div class="experienceHeader">
            <div class="titleLogo">
                <img class="ms-5" src="../assets/img/logo-restaurant-2x-600x115.png" width="250" alt="">
            </div>

            <div class="testo mx-auto text-light">
                <div class="d-flex">



                    <span>----</span>
                    <p class="text-uppercase">the best table in town</p>



                </div>    

                <div>
                    <h1 class="text-uppercase">fine dining experience</h1>
                    <br>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <br>
                    <button class="bottone text-uppercase text-light">explore the menu</button>
                </div>
            </div>
            
        </div>

        <div class="imgHeader">
                <ul class="titleLogo d-flex gap-4 justify-content-center p-4 my-1 text-light">
                    <li v-for="(element, index) in headerAvada" :key="index">
                        {{ element.nome }}
                    </li>
                </ul>
            <!-- <img src="../assets/img/slider52x.jpg" alt=""> -->
        </div>
    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    ul{
        list-style-type: none;
    }

    header{

        .experienceHeader{
            width: 47%;
            background-color: black;
            height: 95vh;

            .testo{
                width: 350px;
                padding: 20px;
                margin-top: 100px;
            }

            .bottone{
                border: 1px solid white;
                background-color: transparent;
                padding: 10px;
                width: 55%;
            }
        }

        .imgHeader{
            background-image: url('../assets/img/slider52x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 53%;
            height: 95vh;
            margin: 0;
        }

        .titleLogo{
                padding: 20px;
        }
    }
</style>

