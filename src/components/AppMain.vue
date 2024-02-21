<script>
    import UniversalExperience from './main/UniversalExperience.vue'
    import AppCritics from './main/Critics.vue'
    import LatestNews from './main/LatestNews.vue'
    import Menu from './main/Menu.vue'

    export default{
        name: "AppMain.vue",
        components:{
            UniversalExperience,
            AppCritics,
            LatestNews,
            Menu,
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <UniversalExperience/>
    <AppCritics/>
    <LatestNews/>
    <Menu/>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

</style>
