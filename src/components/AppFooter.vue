<script>
    import Social from './footer/Social.vue'

    export default{
        name: "AppFooter.vue",
        components:{
            Social
        },
        data(){
            return{
                social:[
                    {
                        facebook:'<i class="fa-brands fa-facebook-f"></i>'
                    },
                    {
                        twitter:'<i class="fa-brands fa-x-twitter"></i>'
                    },
                    {
                        youtube:'<i class="fa-brands fa-youtube"></i>'
                    },
                    {
                        instagram:'<i class="fa-brands fa-instagram"></i>'
                    },
                    {
                        linkedin:'<i class="fa-brands fa-linkedin-in"></i>'
                    }
                ]
            }
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>


    <header>
        <figure class="imgKunPaoChicken">
            <!-- <img src="../assets/img/slider52x.jpg" alt=""> -->
            <div class="testo d-flex flex-column">

                <div>
                    <h4>img avada</h4>
                </div>
                <p>Quam eu proin sit massa condimentum. Volutpat non pulvinar <br> aliquet nune. Quam eu proin sit massa condimentum.</p>



                <Social/>


                
                    <div class="social d-flex gap-5 justify-content-center">
                        <div v-for="(element, index) in social" :key="index" v-html="element[Object.keys(element)[0]]"></div>      

                    </div>


            </div>





                <!-- 
                <div class="social d-flex gap-5 justify-content-center">

                    <div>facebook</div>   <i class="fa-brands fa-facebook-f"></i> 
                    <div>twitter</div>   <i class="fa-brands fa-x-twitter"></i>
                    <div>youtube</div>   <i class="fa-brands fa-youtube"></i>
                    <div>instagram</div> <i class="fa-brands fa-instagram"></i>
                    <div>linkedin</div>   <i class="fa-brands fa-linkedin-in"></i>

                </div>
                 -->

        </figure>

        <div class="copyright text-light p-3 text-center">
            <p>&copy; Copyright 2012 - 2024 &VerticalSeparator; <span>Avada Website Builder</span> <span>by ThemeFusion</span> &VerticalSeparator; All Right Reserved &VerticalSeparator; Powered by <span>WordPress</span></p>
        </div>

    </header>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

header{

    .imgKunPaoChicken{

        position: relative;
        background-image: linear-gradient(0deg, rgba(0,0,0,0) 0%, rgba(0,0,0,1) 100%), url('../assets/img/slider52x.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 500px;
        margin: 0px;

        .testo{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            color: white;
        }

        .social{

            div{
                background-color: white;
                color: black;
                border-radius: 50%;
                padding: 12px;
            }
        }
    }

    .copyright{
        background-color: black;

        p{
            color: #707070;

            span{
                color: white;
            }
        }
    }

}
</style>
