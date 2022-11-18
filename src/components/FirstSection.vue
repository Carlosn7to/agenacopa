<template>
  <div  :style="{ backgroundImage: 'url(' + require('@/assets/img/BG-1.png') + ')' }">
    <img :src="require('@/assets/img/SELO.png')" alt="jogador">
    <button>Conecte-se à Copa do Mundo</button>

  </div>
</template>

<script>
export default {
  name: "FirstSection"
}
</script>

<style scoped lang="scss">

div {
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;

  img:nth-child(1) {
    width: 50%;
    height: auto;
    display: block;
    margin: 0 auto;
    padding-top: 5vh;
  }

  button {
    margin: 0 auto;
    display: block;
    position: relative;
    bottom: -3vh;
    background-color: #F9AC06;
    color: #E4370C;

    font-size: 2.6rem;
    letter-spacing: .6px;
    font-weight: 800;

    border: none;
    border-radius: 13px;

    padding: 20px 35px;
    cursor: pointer;
  }
}

</style>