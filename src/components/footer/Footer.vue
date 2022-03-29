<template>
    <footer>
        <FooterNav/>
        <FooterSocial/>
    </footer>
</template>

<script>
import FooterNav from './FooterNav.vue'
import FooterSocial from './FooterSocial.vue'

export default {
    name:"FooterWrap",
    components:{
        FooterNav,
        FooterSocial,
    }
}
</script>

<style>

</style>