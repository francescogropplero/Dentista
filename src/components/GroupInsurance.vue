<template>
  <div class="flex flex-wrap mt-28">
    <TheInsurance :img="imageUrl" name="Nome Assicurazione" />
    <TheInsurance :img="imageUrl" name="Nome Assicurazione" />
  </div>
</template>

<script>
import TheInsurance from "./TheInsurance.vue";
import insurance from "@/assets/img/insurance.jpg";

export default {
  data() {
    return {
      myElement: null,
      imageUrl: insurance,
    };
  },
  components: {
    TheInsurance,
  },
  mounted() {
    this.myElement = true;
  },
};
</script>

<style scoped>
div {
  width: 50%;
  margin: 0 auto;
}
@media (max-width: 1361px) {
  div {
    margin-left: 20vw !important;
  }
}
</style>
