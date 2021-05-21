<template>
  <div id="app">
    <Header :menu="links" />
    <Jumbotron />
    <Main />
    <Bonus />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Bonus from './components/Bonus.vue'
import Jumbotron from './components/Jumbotron.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  data(){
    
    return{
      links:[
        {
          text:'characters',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'comics',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'movies',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'tv',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'games',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'collectibles',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'videos',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'fans',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'news',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text:'shop',
          url: 'javascript:void(0)',
          current: false
        },
      ]
    }
  },
  components: {
    Header,
    Main,
    Bonus,
    Jumbotron,
    Footer
  }
}
</script>

<style lang="scss">
  @import './assets/style/general.scss';
  @import './assets/style/utilities.scss';
  
</style>
