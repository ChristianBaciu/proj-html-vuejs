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
        <div class="experienceHeader">
            <div class="titleLogo">
                <img class="ms-5" src="../assets/img/logo-restaurant-2x-600x115.png" width="250" alt="">
            </div>

            <div class="dining mx-auto text-light">
                <div class="barra pe-5">
                    <span></span>
                    <h5>the best table in town</h5>
                </div>    

                <div class="testo">
                    <h1>fine dining experience</h1>
                    <br>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <br>
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

        .experienceHeader{
            background-color: black;
            width: 47%;
            height: 95vh;

            .dining{
                width: 400px;
                margin-top: 100px;

                .testo{
                    padding-top: 35px;
                    margin-left: 10px;
                    padding-left: 47px;
                }

                .barra{
                    display: flex;
                    align-items: center;

                    span{
                        background-color: white;
                        width: 40px;
                        height: 1px;
                        margin-right: 20px;
                    }

                    h5{
                        margin: 0;
                    }
                }
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

            ul{
                list-style-type: none;
            }
        }

        .titleLogo{
            padding: 20px;
        }
    }
</style>

