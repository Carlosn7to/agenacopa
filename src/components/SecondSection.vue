<template>
  <div id="section-2" :style="{ backgroundImage: 'url(' + require('@/assets/img/texture_orange.png') + ')' }">
    <h1 style="color: #fff">Confira a escalação da Seleção FIBRA!</h1>
    <h1 style="color: #FFC222">COMBOS de Internet+TV.</h1>
    <br>
    <br>
    <div class="cards">
      <img :src="require('@/assets/img/740.png')" alt="">
      <img :src="require('@/assets/img/480.png')" alt="" style="width: 22vw">
      <img :src="require('@/assets/img/1GB.png')" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "SecondSection"
}
</script>

<style scoped lang="scss">

#section-2 {
  width: 100vw;
  background-size: cover;
  padding: 5vh 0vw;



  h1 {
    text-align: center;
    font-size: 2.8rem;
    font-weight: 800;
  }


  .cards {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1vw ;
    img {
      width: 19vw;
      height: auto;
      cursor: pointer;

    }
  }

}

</style>