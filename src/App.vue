<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Jumbotronmain />
    <Products />
    <Main /> 
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Jumbotronmain from './components/Jumbotronmain.vue'
import Products from './components/Products.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Jumbotronmain,
    Products,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">

   
</style>
