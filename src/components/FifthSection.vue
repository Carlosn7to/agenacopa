<template>
  <div id="section-5" :style="{ backgroundImage: 'url(' + require('@/assets/img/BG.png') + ')' }">
    <form action="#">
      <p>Quero internet 100% FIBRA + 70 CANAIS DE TV</p>
      <div class="inputs">
        <input type="text" name="name" id="name" placeholder="Nome" autocomplete="off">
        <input type="text" name="email" id="email" placeholder="E-mail" autocomplete="off">
        <input type="text" name="tel" id="tel" placeholder="Telefone" autocomplete="off">
        <input type="submit" value="ENVIAR">
      </div>
    </form>
    <div class="player-sport">
      <img :src="require('@/assets/img/SELO SPORTV.png')" alt="">
      <img :src="require('@/assets/img/JOGADOR.png')" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "FifthSection"
}
</script>

<style scoped lang="scss">

#section-5 {
  width: 100%;
  height: 60vh;

  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;

  form {
    background-color: #18183C;
    width: 25vw;
    border-radius: 15px;
    position: relative;
    top: -5vh;
    padding: 4vh 2vw 8vh 2vw;

    p {
      color: #fff;
      font-size: 1.8rem;
      font-weight: 800;
      text-align: center;
    }

    .inputs {
      display: flex;
      flex-direction: column;
      gap: 2vh;
      margin-top: 3vh;

      input[type=text] {
        height: 7vh;
        border-radius: 5px;
        border: none;
        padding: 0 15px;
        outline: none;
      }

      input[type=submit] {
        padding: 10px 0;
        background-color: #EF3A29;
        color: #fff;
        border: none;
        border-radius: 5px;
        font-weight: 800;
        cursor: pointer;
        transition: .2s ease;

        &:hover {
          color: #EF3A29;
          background-color: #fff;
        }
      }
    }
  }

  .player-sport {
    display: flex;
    align-items: center;
    position: relative;
    top: -5vh;

    img:nth-child(1) {
      position: relative;
      width: 10vw;
      left: 17%;
      z-index: 1;
    }

    img:nth-child(2) {
      position: relative;
      right: 10%;
      width: 20vw;
      z-index: 2;
    }
  }
}

</style>