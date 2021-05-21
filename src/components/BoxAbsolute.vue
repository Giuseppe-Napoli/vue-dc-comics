<template>
  <div>
    <h2>current series</h2>
  </div>
</template>

<script>
export default {
name: 'BoxAbsolute'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';
  div{
    position: absolute;
    top: - 25px;
    left: 10%;
    h2{
      color: white;
      text-transform: uppercase;
      padding: 8px 25px;
      background-color: $colorBrand;
    }
  }
</style>