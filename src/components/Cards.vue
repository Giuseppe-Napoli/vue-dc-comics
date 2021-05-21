<template>
  <div class="box">
    <div class="box-img">
      <img :src="card.thumb" alt="">
    </div>
    <h4>{{card.series}}</h4>
  </div>
</template>

<script>
export default {
  name: 'Cards',
  props:{
    card: Object
  }
}
</script>

<style lang="scss" scoped>

  .box{
    padding: 10px;
    margin-bottom: 20px;
    flex-basis: calc(100% / 6);
    h4{
      color: white;
      text-transform: uppercase;
      font-size: 15px;
      font-weight: 400;
    }
    .box-img{
        height: 200px;
        overflow: hidden;
        margin-bottom: 10px;
    }
  }
</style>