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
                        nome: '<i class="fa-solid fa-cart-shopping"></i>'
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
        <div class="textExperience">
            <div class="titleLogo">
                <img class="ms-5" src="../assets/img/logo-restaurant-2x-600x115.png" width="250" alt="">
            </div>

            <div class="dining mx-auto text-light">

                <div class="separatore d-flex align-items-center">
                    <div class="barra"></div>
                    <h5>fine dining experience</h5>
                </div>    

                <div class="info">
                    <h1>fine dining experience</h1>
                    <p class="my-5">Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <button class="button-black">explore the menu</button>
                </div>
            </div>
        </div>

        <div class="imgHeader">
            <ul class="titleLogo d-flex gap-4 justify-content-center p-4 my-1 text-light">
                <li v-for="(element, index) in headerAvada" :key="index">
                    <span v-if="element.nome.includes('<i')" v-html="element.nome"></span>
                    <span v-else>{{ element.nome }}</span>
                </li>
            </ul>
            <!-- <img src="../assets/img/slider52x.jpg" alt=""> -->
        </div>
    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    header{

        .textExperience{
            background-color: black;
            width: 47%;
            height: 100vh;

            .dining{
                width: 400px;
                margin-top: 100px;

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

        .imgHeader{
            background-image: url('../assets/img/slider52x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 53%;
            height: 100vh;
            margin: 0;

            ul{
                list-style-type: none;
            }
        }

        .titleLogo{
            padding: 20px;
        }
    }
</style>

