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

<template>
    <header class=" bg-dark text-light">

        <div class="d-flex justify-content-around align-items-center">
            <figure>
                <img src="../assets/img/logo-restaurant-2x-600x115.png" alt="">
            </figure>

            
            <ul class="d-flex gap-5">
                <li v-for="(element, index) in headerAvada" :key="index">
                    {{ element.nome }}
                </li>
            </ul>
        </div>

        <main class="d-flex justify-content-between">
            <div class="experience">

                <p>the best table in town</p>

                <div class="mx-auto">
                    <h1>fine dining experience</h1>

                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>

                    <button>explore the menu</button>
                </div>

            </div>

            <figure>
                <!-- <img src="../assets/img/slider52x.jpg" alt=""> -->
            </figure>
            
        </main>
    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    ul{
        list-style-type: none;
    }

    main{
        
        .experience{
            width: 40%;
            background-color: red;

            div{
                background-color: orange;
                width: 300px;
            }

        }

        figure{
            background-image: url('../assets/img/slider52x.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            width: 60%;
            height: 75vh;
        }
    }

</style>

