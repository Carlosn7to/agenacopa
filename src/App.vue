<template>
    <section>
      <FirstSection/>
    </section>
    <section>
      <SecondSection/>
    </section>
    <section>
      <ThirdSection/>
    </section>
    <section>
      <FourSection/>
    </section>
    <section>
      <FifthSection/>
    </section>
    <section>
      <SixthSection/>
    </section>
    <footer>
      <FooterComponent/>
    </footer>
</template>

<script>

import FirstSection from "@/components/FirstSection";
import SecondSection from "@/components/SecondSection";
import ThirdSection from "@/components/ThirdSection";
import FourSection from "@/components/FourSection";
import FifthSection from "@/components/FifthSection";
import SixthSection from "@/components/SixthSection";
import FooterComponent from "@/components/FooterComponent";

export default {
  name: 'App',
  components: {
    FirstSection,
    SecondSection,
    ThirdSection,
    FourSection,
    FifthSection,
    SixthSection,
    FooterComponent
  }
}
</script>

<style lang="scss">
*, ::after, ::before {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'TT Hoves', sans-serif;

  @font-face {
    font-family: "TT Hoves";
    src: local("TT Hoves"), url(./fonts/TThover/TTHoves-ExtraBold.ttf);
  }

}

html {
  font-size: 62.5%;
  background-repeat: repeat;
  overflow-x: hidden;
}

#app {
  width: 100vw;
  height: 100vh;
  section:nth-child(1) {
    width: 100vw;
  }
}

/*   SCROLL BAR   */
::-webkit-scrollbar-track {
  background-color: #F4F4F4;
}
::-webkit-scrollbar {
  width: 6px;
  background: #F4F4F4;
}
::-webkit-scrollbar-thumb {
  background: #dad7d7;
}
</style>
