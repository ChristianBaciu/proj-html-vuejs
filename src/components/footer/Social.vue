<script>
    export default{
        name: "Social.vue",
        props:{
            propsSocial: 'Array'
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <div class="social d-flex gap-3 justify-content-center">
        <div v-for="(icon, index) in propsSocial" :key="index" v-html="icon"></div>
    </div>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
header{

    .social{

        div{
            background-color: white;
            color: black;
            border-radius: 50%;
            padding: 12px;
            padding-left: 15px;
            padding-right: 15px;
            transition: all 0.5s ease 0s;
            width: 50px;
            height: 50px;

            &:hover{
                transition: all 0.5s ease 0s;
                background-color: black;
                color: white;
            }
        }
    }
}

</style>
