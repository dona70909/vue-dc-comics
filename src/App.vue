<template>
  <div id="app">
    <Header/>
    <MainContent/>
    <MainContentMenu/>
    <Footer/>
  </div>
</template>

<script>

import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import MainContentMenu from './components/MainContentMenu.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    MainContentMenu,
    Footer,

  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.padding{
  padding: 0 8rem;
}

.d-flex{
  display: flex;
}
</style>
