<template>
  <div id="section-3">
    <h1>Qualquer um dos três planos te dão acesso ao DIRECTV GO!</h1>
    <img :src="require('@/assets/img/LOGO DGO.png')" alt="">
    <div class="cards">
      <img :src="require('@/assets/img/BOTÃO CANAIS.png')" alt="">
      <img :src="require('@/assets/img/BOTÃO TELAS.png')" alt="">
      <img :src="require('@/assets/img/BOTÃO CANAIS.png')" alt="">
      <img :src="require('@/assets/img/BOTÃO FILMES.png')" alt="">
      <img :src="require('@/assets/img/BOTÃO CANAIS ESPORTES.png')" alt="">
      <img :src="require('@/assets/img/BOTÃO ACESSO.png')" alt="">
    </div>
    <div class="tv-direct">
      <img :src="require('@/assets/img/TV MOCKUP.png')" alt="">
      <img :src="require('@/assets/img/MULHER.png')" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "ThirdSection"
}
</script>

<style scoped lang="scss">

#section-3 {
  display: flex;
  align-items: center;
  flex-direction: column;
  background-color: #18183C;
  padding: 5vh 1vw;
  gap: 5vh;

  h1 {
    font-size: 2rem;
    color: #fff;
    font-weight: 700;
  }

  img {
    width: 15vw;
    height: auto;
  }

  .cards {
    display: grid;
    grid-template-columns: 18vw 18vw 18vw;
    flex-wrap: wrap;
    gap: 2vw;
    padding: 0 10%;

    img {
      width: 100%;
      height: auto;
      display: block;
      margin: 0 auto;
    }
  }

  .tv-direct {
    width: 100%;
    padding: 0 0 0 20%;
    img:nth-child(1) {
      width: 40vw;
      height: auto;

    }

    img:nth-child(2) {
      width: 24vw;
      height: auto;
      position: relative;
      right: 10%;
      bottom: -5.5vh;
    }
  }
}

@media (max-width: 360px) {
  #section-3 {
    gap: 3vh;

    
    h1 {
      font-size: 1.6rem;
    }

    img {
      width: 26vw;
    }

    .cards {
      grid-template-columns: 27vw 27vw 27vw;
    }

    .tv-direct {
      padding: 0 0 0 6%;

      img:nth-child(1) {
        width: 50vw;
      }

      img:nth-child(2) {
        width: 35vw;
      }
    }


  }
}
</style>