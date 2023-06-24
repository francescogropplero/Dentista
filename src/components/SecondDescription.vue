<template>
  <section id="assicurazioni" :class="{ 'slide-in': myElement }">
    <h2>Parliamo di inclusività.</h2>
    <p>
      Al fine di fornire un servizio di prima <br />
      qualità accessibile a chiunque, abbiamo <br />
      stretto convenzioni e collaborazioni con <br />
      vari enti assicurativi:<br />
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
  margin-top: 10vh;
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
    margin-top: 1rem !important;
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
