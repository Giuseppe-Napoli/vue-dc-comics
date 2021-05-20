<template>
  <div id="app">
    <Header />
    <Main />
    <Bonus />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Bonus from './components/Bonus.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Bonus,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/general.scss';
  @import './assets/style/utilities.scss';
  
</style>
