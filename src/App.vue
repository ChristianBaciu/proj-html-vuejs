<script>
    import AppHeader from './components/AppHeader.vue'
    import UniversalExperience from './components/main/UniversalExperience.vue'
    import AppCritics from './components/main/AppCritics.vue'
    import LatestNews from './components/main/LatestNews.vue'

    export default{
        components:{
            AppHeader,
            UniversalExperience,
            AppCritics,
            LatestNews,
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <AppHeader/>

    <main>
        <UniversalExperience/>
        <AppCritics/>

        <LatestNews/>
    </main>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    @use './scss/styles.scss';
</style>
