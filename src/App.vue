<template>
  <div id="app">
    <Header/>
    <MainContent/>
    <MainContentMenu/>
    <Footer/>
    <FooterSignUp/>
  </div>
</template>

<script>

import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import MainContentMenu from './components/MainContentMenu.vue'
import Footer from './components/Footer.vue'
import FooterSignUp from './components/FooterSignUp.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    MainContentMenu,
    Footer,
    FooterSignUp,

  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  min-width: 1200px;
}

.padding{
  padding: 0 8rem;
}

.d-flex{
  display: flex;
}

.position-relative{
  position: relative;
}

ul{
  list-style: none;
}

a{
  text-decoration: none;
}
</style>
