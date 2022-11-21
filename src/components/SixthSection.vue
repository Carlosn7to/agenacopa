<template>
  <div id="section-6">
    <div class="text">
      <h1>Tire suas dúvidas:</h1>
      <div class="content">
        <h1>Quantos aparelhos podem estar conectados ao DGO?</h1>
        <p>Simultaneamente apenas 2 aparelhos. Mas até 5 podem ficar logados na mesma conta.</p>
      </div>
      <div class="content">
        <h1>Quais as formas de pagamento que aceitamos?</h1>
        <p>
          Pagamento em débito em conta disponível nos bancos Santander e Caixa Econômica Federal.
          Para correntistas dos demais bancos, os meios de pagamento disponíveis são
          apenas boleto e cartão de crédito(bandeiras Mastercard, Visa, Cielo, American Express,
          Elo, Diners Club, Agiplan, Banes Card, Hipercard, JCB, Credz)
        </p>
      </div>
      <div class="content">
        <h1>Quanto custa a instalação?</h1>
        <p>A instalação é gratuíta e sem taxas.</p>
      </div>
    </div>
    <button>TEM OUTRAS DÚVIDAS? CLIQUE AQUI.</button>
  </div>
</template>

<script>
export default {
  name: "SixthSection"
}
</script>

<style scoped lang="scss">

#section-6 {
  width: 100%;
  background-color: #0F297D;
  padding: 8vh 20vw;

  .text {
    display: flex;
    flex-direction: column;
    gap: 3vh;
    h1 {
      font-size: 2rem;
      color: #ffffff;
      font-weight: 800;
    }

    .content {
      display: flex;
      flex-direction: column;
      gap: 2vh;
      width: 70%;
      h1 {
        font-weight: 600;
      }

      p {
        color: #ABAFCA;
        font-size: 1.2rem;
      }
    }


  }
  button {
    color: #fff;
    background-color: #EF3A29;
    padding: 10px 20px;
    border: none;
    outline: none;
    margin: 4vh 0 0 0;
    border-radius: 5px;
    font-weight: 800;
    letter-spacing: .4px;
    cursor: pointer;
    transition: .2s ease;
    box-shadow: rgba(9, 30, 66, 0.25) 0px 4px 8px -2px, rgba(9, 30, 66, 0.08) 0px 0px 0px 1px;

    &:hover {
      color: #EF3A29;
      background-color: #fff;
    }
  }
}

</style>