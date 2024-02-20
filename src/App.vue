<script>
    import AppHeader from './components/AppHeader.vue'
    import AppMain from './components/main/AppMain.vue'
    import BestInTown from './components/main/BestInTown.vue'

    export default{
        components:{
            AppHeader,
            AppMain,
            BestInTown
        }
    }
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <AppHeader/>

    <main>
        <AppMain/>
        <BestInTown/>
    </main>
    
</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
    @use './scss/styles.scss';
</style>
