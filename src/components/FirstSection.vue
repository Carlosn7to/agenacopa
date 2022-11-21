<template>
  <div id="section-1" :style="{ backgroundImage: 'url(' + require('@/assets/img/BG-1.png') + ')' }">
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

#section-1 {
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;

  img:nth-child(1) {
    width: 50%;
    height: auto;
    display: block;
    margin: auto;
    position: relative;
    top: 13vh;
  }

  button {
    margin: 0 auto;
    display: block;
    position: relative;
    bottom: -3vh;
    background-color: #F9AC06;
    color: #E4370C;
    box-shadow: rgba(9, 30, 66, 0.25) 0px 4px 8px -2px, rgba(9, 30, 66, 0.08) 0px 0px 0px 1px;
    transition: .2s ease;
    &:hover {
      color: #F9AC06;
      background-color: #E4370C;
    }

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