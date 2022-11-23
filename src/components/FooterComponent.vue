<template>
  <div id="footer">
    <div class="text-content">
      <h1>Conheça outras ofertas <br> em nossas redes</h1>

      <div class="socials">
        <img :src="require('@/assets/img/insta.png')" alt="">
        <img :src="require('@/assets/img/facebook.png')" alt="">
        <img :src="require('@/assets/img/youtube.png')" alt="">
        <img :src="require('@/assets/img/whatsapp.png')" alt="">
      </div>

      <p>
        Permanência mínima de 12 meses. Multa fidelidade de R$950,00 (pro rata), podendo também ser adquirido
        sem permanência mínima nos termos do regulamento. Pagamento em débito em conta disponível nos bancos
        Santander e Caixa Econômica Federal. Para correntistas dos demais bancos, os meios de pagamento disponíveis
        são apenas boleto e cartão de crédito (bandeiras Mastercard, Visa, Cielo, American Express, Elo, Diners Club,
        Agiplan, Banes Card, Hipercard, JCB, Credz). Sem taxa de instalação. Equipamentos em locação. Não é possível
        realizar downgrade nos 3 primeiros meses. Consulte disponibilidade dos serviços, valores, regulamento de
        ofertas, contrato de permanência e mais informações em: https://www.agetelecom.com.br.
      </p>
    </div>
    <div class="logo">
      <img :src="require('@/assets/img/LOGO AGE RODAPÉ.png')" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent"
}
</script>

<style scoped lang="scss">

#footer {
  width: 100%;
  height: 50vh;
  background-color: #18183C;
  padding: 3% 20%;
  display: flex;
  align-items: center;

  .text-content {
    width: 80%;
    h1 {
      color: #fff;
      font-weight: 800;
      font-size: 2rem;
    }

    .socials {
      margin: 2vh 0;
      display: flex;
      align-items: center;
      gap: .5vw;
    }

    p {
      color: #ffffff;
      width: 70%;
      text-align: justify;
    }
  }
}


@media (max-width: 360px) {
  #footer {
    height: initial;
  }
}
</style>