<template>
  <div class="banner">
    <ul>
      <li>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
        <h2>digital comics</h2>
      </li>
      <li>
        <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
        <h2>dc merchandise</h2>
      </li>
      <li>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
        <h2>subscriptions</h2>
      </li>
      <li>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator">
        <h2>comics shop locator</h2>
      </li>
      <li>
        <img class="special-img" src="../assets/img/buy-dc-power-visa.svg" alt="power visa">
        <h2>dc power visa</h2>
      </li>


    </ul>
  </div>
</template>

<script>
export default {
  name: 'Bonus',
}
</script>

<style lang="scss" scoped>
  
  @import '../assets/style/vars.scss';


  .banner{
    background-color: $colorBrand;
    padding: 60px 0px;
  }
  
  ul{
    display: flex;
    justify-content: space-evenly;
    width: 70%;
    align-items: center;
    margin: 0 auto;
  }

  li{
    display: flex;
    align-items: center;
    cursor: pointer;
    img{
      max-width: 50px;
      max-height: 40px;
      margin-right: 8px;
    }
    .special-img{
      width: 40px;
    }
    h2{
      color: white;
      text-transform: uppercase;
      font-size: 16px;
      font-weight: 300;
    }
  }

</style>