<template>
  <div class="flex flex-wrap ml-auto mt-60">
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="imageUrl"
      name="Stea Cecilia"
      job="Odontoiatra"
    />
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="image2Url"
      name="Rulfo Angela"
      job="Odontoiatra"
    />
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="imageUrl"
      name="Di Caccamo Stella"
      job="Collaboratrice"
    />
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="image3Url"
      name="Oliva Marco"
      job="Collaboratore"
    />
  </div>
</template>

<script>
import ThePerson from "./ThePerson.vue";
import CeciliaStea1 from "@/assets/img/CeciliaStea1.jpg";
import donna from "@/assets/img/donna.jpg";
import ragazzo from "@/assets/img/ragazzo.jpg";

export default {
  data() {
    return {
      myElement: null,
      imageUrl: CeciliaStea1,
      image2Url: donna,
      image3Url: ragazzo,
    };
  },
  components: {
    ThePerson,
  },
  mounted() {
    this.myElement = true;
  },
};
</script>

<style scoped>
div {
  width: 50%;
}
@keyframes slideIn {
  0% {
    transform: translateY(-10%);
  }
  100% {
    transform: translateY(0);
  }
}
.slide-in {
  animation: slideIn 1.3s ease-out;
}
@media (max-width: 1361px) {
  div {
    margin-left: 20vw !important;
    margin-top: 5rem !important;
  }
}
</style>
