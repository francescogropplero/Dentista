<template>
  <div class="padre mt-14">
    <div class="logo">
      <TheLogo />
    </div>
    <div class="flex justify-center">
      <div
        ref="myElement"
        :class="[
          'nav',
          'ml-40',
          'px-20',
          'justify-center',
          { 'slide-in': myElement },
        ]"
      >
        <a
          class="link"
          v-for="(item, index) in navLinks"
          :key="index"
          href="#"
          >{{ item }}</a
        >
      </div>
    </div>
  </div>
</template>

<script>
import TheLogo from "./TheLogo.vue";

export default {
  data() {
    return {
      myElement: null,
      navLinks: ["Home", "Chi siamo", "Assicurazioni", "Contatti"],
    };
  },
  components: {
    TheLogo,
  },
  mounted() {
    this.myElement = true;
  },
};
</script>

<style scoped>
a {
  font-family: "SF Semibold";
  font-size: 1.1rem;
  letter-spacing: 0.5px;
}
.logo {
  height: 8vh;
  width: 12.5vw;
  margin-left: -25vw;
}
.padre {
  display: flex;
  justify-content: center;
}
.nav {
  display: flex;
  background-color: #ffffff;
  align-items: center;
  border-radius: 25px;
}
.nav > *:not(:first-child) {
  margin-left: 30px;
}
@keyframes slideIn {
  0% {
    transform: translateY(-100%);
  }
  100% {
    transform: translateY(0);
  }
}
.slide-in {
  animation: slideIn 0.9s ease-out;
}

/* Media Queries */
@media (max-width: 635px) {
  .padre {
    display: none !important;
  }
}
</style>
