<template>
  <div>
      <div class="background-second"></div>
      <div class="landing-pages">
        <LandingFirstPage/>
        <LandingSecondPage/>
        <Footer/>
      </div>
  </div>
</template>

<script>
import LandingFirstPage from "../components/LandingFirstPage.vue";
import LandingSecondPage from "../components/LandingSecondPage.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "Main",
  components: {
    LandingFirstPage,
    LandingSecondPage,
    Footer
  }
};
</script>

<style scoped>
.landing-pages {
    display: flex;
    flex-direction: column;
}

.background-second {
    position: absolute;
    width: 100%;
    height: 900px;
    margin: 900px 0 0 0;
    background: var(--primary-main);;
    z-index: -1;
}
</style>
