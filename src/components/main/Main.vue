<template>
    <main>
        <MainJumbo/>
        <MainCards/>
        <MainNav/>
    </main>
</template>

<script>
import MainJumbo from './MainJumbo.vue'
import MainCards from './MainCards.vue'
import MainNav from './MainNav.vue'

export default {
    name:"MainWrapper",
    components:{
        MainJumbo,
        MainCards,
        MainNav,
    }
}
</script>

<style lang="scss">

</style>