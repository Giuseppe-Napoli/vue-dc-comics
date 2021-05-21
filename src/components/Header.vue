<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="Logo">
    <nav>
      <ul>
        <li v-for="(link, index) in menu" 
        @click="changeActive(index)"
        :key="index">
          <a :class="{'active': link.current}" :href="link.url">{{ link.text}}</a>
        </li>
        <!-- <li><a href="/">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">videos</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li> -->
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name:'Header',
  props:{
    menu: Array
  },
  data(){
    return{
      links:[],
    }
  },
  methods:{
    changeActive(index){
      this.menu.forEach((link)=>{
        link.current = false
      })
      this.menu[index].current = true
    }
  },
}
</script>

<style  lang="scss" scoped>
  
  @import '../assets/style/vars.scss';

  header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 150px;
  }
  
  ul{
    li{
      display: inline-block;
      padding: 0 10px;
      a{
        text-transform: uppercase;
        font-size: 13px;
        font-weight: 600;
        color: #464646;
        &:hover,
        &.active{
          color: #0C7CEC;
          border-bottom: 5px solid $colorBrand;
          padding-bottom: 62px;
        }
      }
    }
  }
</style>