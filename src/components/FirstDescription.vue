<template>
  <section id="chi-siamo" :class="{ 'slide-in': myElement }">
    <h2>La tua dentista nel monregalese.</h2>
    <p>
      Il benessere dei pazienti è al centro <br />del nostro impegno da più di
      20 anni. <br />
      E tutto questo non sarebbe possibile <br />
      se al nostro fianco non avessimo <br />
      persone <span>FANTASTICHE</span>
    </p>
  </section>
</template>

<script>
export default {
  data() {
    return {
      myElement: null,
    };
  },
  mounted() {
    this.myElement = true;
  },
};
</script>

<style scoped>
section {
  margin-left: 7vw;
  margin-top: 15vh;
}
h2 {
  font-family: "SF Semibold";
  font-size: 2.5rem;
}
p {
  font-size: 1.2rem;
  letter-spacing: 0.4px;
}
span {
  margin-left: 2px;
  color: var(--rosa);
  font-family: "SF Bold";
  letter-spacing: 0 !important;
  font-size: 1.8rem;
}
.slide-in {
  animation: slideIn 1.3s ease-out;
}
@keyframes slideIn {
  0% {
    transform: translateX(10%);
  }
  100% {
    transform: translateX(0);
  }
}
@media (max-width: 430px) {
  section {
    margin-top: 12rem !important;
    text-align: center;
    margin-left: 0;
  }
  h2 {
    font-size: 1.5rem;
  }
  p {
    font-size: 1.1rem;
  }
  span {
    font-size: 1.1rem !important;
  }
}
</style>
