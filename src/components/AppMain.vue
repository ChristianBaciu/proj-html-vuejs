<script>
    import UniversalExperience from './main/UniversalExperience.vue'
    import AppCritics from './main/Critics.vue'
    import LatestNews from './main/LatestNews.vue'

    export default{
        name: "AppMain.vue",
        components:{
            UniversalExperience,
            AppCritics,
            LatestNews,
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <UniversalExperience/>
    <AppCritics/>
    <LatestNews/>
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

</style>
