<template>
  <div :style="{ backgroundImage: 'url(' + require('@/assets/img/texture_orange.png') + ')' }">
    <h1 style="color: #fff">Confira a escalação da Seleção FIBRA!</h1>
    <h1 style="color: #FFC222">COMBOS de Internet+TV.</h1>
    <img :src="require('@/assets/img/logo.png')" alt="">
  </div>
</template>

<script>
export default {
  name: "SecondSection"
}
</script>

<style scoped lang="scss">

div {
  width: 100vw;
  background-size: cover;
  padding: 5vh 0vw;



  h1 {
    text-align: center;
    font-size: 2.8rem;
    font-weight: 800;
  }

  img {
    width: 35%;
    height: auto;
    position: relative;
    top: -6vh;
    opacity: .8;
  }

}

</style>