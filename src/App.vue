<script>
    import AppHeader from './components/AppHeader.vue'
    import UniversalExperience from './components/main/UniversalExperience.vue'
    import BestInTown from './components/main/BestInTown.vue'
    import AppCritics from './components/main/AppCritics.vue'

    export default{
        components:{
            AppHeader,
            UniversalExperience,
            BestInTown,
            AppCritics
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <AppHeader/>

    <main>
        <UniversalExperience/>
        <BestInTown/>
        <AppCritics/>
    </main>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    @use './scss/styles.scss';
</style>
