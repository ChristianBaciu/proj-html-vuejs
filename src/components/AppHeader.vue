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
                        nome: 'Culinary',
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
                    // {
                    //     nome: '<i class="fa-solid fa-cart-shopping"></i>'
                    //     // false
                    // }
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

        <!-- <div class="d-flex justify-content-around align-items-center">
            <img class="bg-primary" src="../assets/img/logo-restaurant-2x-600x115.png" width="300" alt="">

            
            <ul class="d-flex gap-5">
                <li v-for="(element, index) in headerAvada" :key="index">
                    {{ element.nome }}
                </li>
            </ul>
        </div> -->



<template>
    <header class="d-flex justify-content-between">

        <div class="experienceHeader">

            <div class="titleLogo">
                <img class="bg-danger" src="../assets/img/logo-restaurant-2x-600x115.png" width="250" alt="">
            </div>

            
            <!-- <div class="mx-auto text-light">

                <div class="mt-5">

                    <p>the best table in town</p>

                </div>    

                <div class="">

                    <h1>fine dining experience</h1>

                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>

                    <button class="btn">explore the menu</button>

                </div>
            </div> -->
        </div>




        <div class="imgHeader">
                <ul class="titleLogo d-flex gap-5 p-4 mt-3 text-light">
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
        .titleLogo{
                width: 100%;
                // background-color: blue;
                padding: 20px;
        }

        .experienceHeader{
            width: 40%;
            background-color: black;
            height: 100vh;
        }

        .imgHeader{
            background-image: url('../assets/img/slider52x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 60%;
            height: 100vh;
            margin: 0;
        }
    }
</style>

