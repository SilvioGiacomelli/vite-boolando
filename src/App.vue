<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Products from '../src/data/db.json'
export default {
  components:{
    Header,
    Main,
    Footer,    
  }
}
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style lang="scss">
@use './assets/scss/main.scss';
</style>
