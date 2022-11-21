<template>
  <div id="section-4">
    <button>QUERO ASSISTIR A COPA AO VIVO</button>
    <div class="club">
      <img :src="require('@/assets/img/LOGO VANTAGENS.png')" alt="">
      <div class="divisor">
        <div></div>
      </div>
      <p>Assine agora qualquer plano de Internet 100% FIBRA e faça parte do <b>Clube de <br> Vantagens AGE.</b>
        Tenha descontos e benefícios diversos serviços e estabelecimentos.
      </p>
      <div class="partners">
        <div class="partner">
          <span>Até 10% OFF</span>
          <img :src="require('@/assets/img/magalu-logo-1.png')" alt="">
        </div>
        <div class="partner">
          <span>10% de desconto</span>
          <img :src="require('@/assets/img/Amazon-Logo.png')" alt="">
        </div>
        <div class="partner">
          <span>Descontos variados</span>
          <img :src="require('@/assets/img/Casas_Bahia_logo_2020.png')" alt="">
        </div>
        <div class="partner">
          <span>10% de desconto</span>
          <img :src="require('@/assets/img/netshoes-logo.png')" alt="">
        </div>
        <div class="partner">
          <span>Até 50% de desconto</span>
          <img :src="require('@/assets/img/cultura inglesa.png')" alt="">
        </div>
        <div class="partner">
          <span>10% de desconto</span>
          <img :src="require('@/assets/img/renner-logo-1-1.png')" alt="">
        </div>
        <div class="partner">
          <span>Até 15% OFF</span>
          <img :src="require('@/assets/img/oticas_2020.png')" alt="">
        </div>
        <div class="partner">
          <span>Até 30% de desconto</span>
          <img :src="require('@/assets/img/BOOKING.png')" alt="">
        </div>
      </div>
      <button>
        <i class="fi fi-brands-whatsapp"></i>
        <span>EU QUERO ENTRAR PARA O CLUBE</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "FourSection"
}
</script>

<style scoped lang="scss">

#section-4 {
  width: 100%;
  background-color: #fff;
  display: flex;
  align-items: center;
  flex-direction: column;
  gap: 5vh;
  padding: 0 0 5vh 0;

  .club {
    display: flex;
    align-items: center;
    flex-direction: column;
    gap: 5vh;
    .divisor {
      width: 100%;
      height: 4px;

      div {
        width: 20%;
        height: 100%;
        margin: 0 auto;
        background-color: #FA7817;
      }
    }

    padding: 0 15vw;
    p {
      font-size: 1.8rem;
      letter-spacing: .6px;
    }

    .partners {
      display: grid;
      gap: 3vw;
      grid-template-columns: 13vw repeat(3, 13vw);
      grid-template-rows: 12vh 12vh;
      width: 100%;

      .partner {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: initial;
        gap: 2vh;

        span {
          color: #FA7411;
          font-size: 1.4rem;
          font-weight: 800;
        }

        img {
          width: 80%;
          display: block;
          margin: 0 auto;
        }
      }
    }

    button {
      background-color: #EF3A29;
      display: flex;
      align-items: center;
      justify-content: initial;
      gap: 1vw;
      padding: 7px 20px;
      margin-top: 4vh;
      cursor: pointer;
      position: relative;
      z-index: 999;

      i {
        font-size: 2rem;
      }
      span {
        font-size: 1.6rem;
        padding: 0 0 5px 0;
      }
    }
  }

  img {
    width: 25vw;
    height: auto;
  }

  button {
    position: relative;
    top: -3vh;
    background-color: #E4370C;
    border-radius: 5px;
    color: #fff;
    font-size: 2rem;
    padding: 12px 45px;
    font-weight: 800;
    cursor: pointer;
    transition: .2s ease;
    border: 2px solid #E4370C;
    box-shadow: rgba(9, 30, 66, 0.25) 0px 4px 8px -2px, rgba(9, 30, 66, 0.08) 0px 0px 0px 1px;


    &:hover {
      color: #E4370C;
      background-color: #fff;
      border: 2px solid #E4370C;
    }
  }

}

</style>