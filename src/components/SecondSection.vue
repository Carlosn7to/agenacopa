<template>
  <div id="section-2" :style="{ backgroundImage: 'url(' + require('@/assets/img/texture_orange.png') + ')' }">
    <h1 style="color: #fff">Confira a escalação da Seleção FIBRA!</h1>
    <h1 style="color: #FFC222">COMBOS de Internet+TV.</h1>
    <br>
    <br>
    <div id="cards-web" class="cards">
      <img :src="require('@/assets/img/740.png')" alt="">
      <img :src="require('@/assets/img/480.png')" alt="" style="width: 22vw">
      <img :src="require('@/assets/img/1GB.png')" alt="">
    </div>
    <div id="cards-mob" class="cards-mob">
      <i class="fi fi-rs-angle-left" @click="tradePlan(0)"></i>
      <div class="plans">
        <img :class="{ '' :   }" :src="require('@/assets/img/740.png')" alt="">
        <img :src="require('@/assets/img/480.png')" alt="">
        <img :src="require('@/assets/img/1GB.png')" alt="">
      </div>
      <i class="fi fi-rs-angle-right" @click="tradePlan(1)"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "SecondSection",
  data () {
    return {
      cards: 1,
      effect: null
    }
  },
  methods: {
    tradePlan: function (action) {

      if(action === 1) {
        if(this.cards === 0) {
          this.effect = 'right'
          return this.cards = 1
        }
        if(this.cards === 1) {
          return this.cards = 2

        }
        if(this.cards === 2) {
          return this.cards = 0

        }
      }

      if(action === 0) {
        if(this.cards === 0) {
          return this.cards = 2

        }
        if(this.cards === 1) {
          return this.cards = 0

        }
        if(this.cards === 2) {
          return this.cards = 1

        }
      }

    }
  }
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
    }

}

@media (max-width: 360px) {

  #section-2 {

    h1 {
      font-size: 2.4rem;
    }

    .cards {
      display: none;
    }

    .cards-mob {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 5vw;

      .plans {
        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden;
        max-width: 40%;


        img {
          width: 40vw;
          height: auto;
          cursor: pointer;

        }
      }

      img {
        width: 40vw;
      }

      i {
        font-size: 7rem;
        color: #18183B;
      }
    }
  }
}

.right {
  animation: right .6s ease-in-out forwards;
}

@keyframes right {
  from {
    transform: translateX(20px);
  }
  to {
    transform: translateX(0);
  }
}

</style>