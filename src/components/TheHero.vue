<template>
  <header :class="['father', { 'slide-in': myElement }]">
    <h1>Un sorriso cambia tutto.</h1>
    <h4 class="item mb-8">La felicità inizia con un sorriso sano.</h4>
    <HomeButton class="btn" style="margin: 0 auto" content="CONTATTACI" />
  </header>
</template>

<script>
import HomeButton from "./HomeButton.vue";

export default {
  data() {
    return {
      myElement: null,
    };
  },
  components: {
    HomeButton,
  },
  mounted() {
    this.myElement = true;
  },
};
</script>

<style scoped>
h1 {
  font-family: "SF Bold";
  font-size: 4rem;
  text-align: center;
}
h4 {
  text-align: center;
  font-size: 1.8rem;
  font-weight: 100;
}
.father {
  margin-top: 2rem;
  width: 100%;
  height: 30vh;
  display: flex;
  flex-direction: column;
  justify-content: center !important;
}

@keyframes slideIn {
  0% {
    transform: translateY(50%);
  }
  100% {
    transform: translateY(0);
  }
}
.slide-in {
  animation: slideIn 1.3s ease-out;
}

@media (max-width: 430px) {
  h1 {
    margin-top: 15rem !important;
    font-size: 3rem;
  }
  h4 {
    font-size: 1.3rem;
  }
}
</style>
