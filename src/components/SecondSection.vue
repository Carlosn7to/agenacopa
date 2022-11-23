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
        <img v-if="cards === 0" :class="{ 'right' : effect === 'right',
                                          'left' : effect === 'left'}" :src="require('@/assets/img/740.png')" alt="">
        <img v-if="cards === 1" :class="{ 'right' : effect === 'right',
                                          'left' : effect === 'left'}" :src="require('@/assets/img/480.png')" alt="">
        <img v-if="cards === 2" :class="{ 'right' : effect === 'right',
                                          'left' : effect === 'left'}" :src="require('@/assets/img/1GB.png')" alt="">
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
          this.effect = 'right'
          return this.cards = 2

        }
        if(this.cards === 2) {
          this.effect = 'right'
          return this.cards = 0

        }
      }

      if(action === 0) {
        if(this.cards === 0) {
          this.effect = 'left'
          return this.cards = 2

        }
        if(this.cards === 1) {
          this.effect = 'left'
          return this.cards = 0

        }
        if(this.cards === 2) {
          this.effect = 'left'
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
  padding: 5vh 0;



  h1 {
    text-align: center;
    font-size: 2.8rem;
    font-weight: 800;
  }


  #cards-web {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1vw ;

    img {
      cursor: pointer;
    }

  }

  #cards-mob {
    display: none;
  }

}

@media (max-width: 360px) {

  #section-2 {

    h1 {
      font-size: 2.4rem;
    }

    #cards-web {
      display: none;
    }

    #cards-mob {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 5vw;

      .plans {
        display: flex;
        align-items: center;
        justify-content: center;



        img {
          width: 45vw;
          min-height: 250px;
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
  animation: right ease-in-out forwards .3s;
}

@keyframes right {
  from {
    opacity: .8;
    transform: translateX(10px);
  }
  to {
    opacity: 1;
    transform: translateX(0px);
  }
}

.left {
  animation: left ease-in-out forwards .3s;
}

@keyframes left {
  from {
    opacity: .8;
    transform: translateX(-10px);
  }
  to {
    opacity: 1;
    transform: translateX(0px);
  }
}


</style>