<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/header/Header.vue'
import Main from './components/main/Main.vue'
import Footer from './components/footer/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
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
