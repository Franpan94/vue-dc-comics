<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Products />
    <Main />
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Products from './components/Products.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Products,
    Main,
    Footer,
    Jumbotron
  }
}
</script>

<style lang="scss">

   
</style>
