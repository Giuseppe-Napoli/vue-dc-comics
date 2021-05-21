<template>
  <main>
    <BoxAbsolute />
    <section class=" container">
      <Cards
        v-for="(product, index) in products"
        :key="index"
        :card="product"
      />
      <button>load more</button>
    </section>
  </main>
</template>

<script>
import products from "@/assets/data/dc-comics.js";
import Cards from "@/components/Cards.vue";
import BoxAbsolute from "../components/BoxAbsolute.vue"
export default {

  name: 'Main',
  components:{
    Cards,
    BoxAbsolute
  },
  data(){
    return{
      products
    }
  },
  mounted(){
    //console.log(comicsDc);
  }

  
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';
  main{
    background-color: #1C1C1C;
    padding: 45px 10px;
    position: relative;
  }
  section{
    display: flex;
    flex-wrap: wrap;
    button{
      color: white;
      text-transform: uppercase;
      margin: 0 auto;
      padding: 10px 50px;
      font-weight: 400;
      background-color:  $colorBrand;
      border: none;
      cursor: pointer;
      &:hover{
        transform: scale(1.1);
      }
    }
  }


</style>