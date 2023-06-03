<template>
  <div :class="['flex', 'flex-wrap', 'ml-auto', 'mt-28']">
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="imageUrl"
      name="Stea Cecilia"
      job="Odontoiatra"
    />
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="image2Url"
      name="Cognome Anna"
      job="Odontoiatra"
    />
    <ThePerson
      :class="[{ 'slide-in': myElement }]"
      :img="imageUrl"
      name="Cognome Stella"
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
import donna2 from "@/assets/img/donna2.jpg";
import donna from "@/assets/img/donna.jpg";
import ragazzo from "@/assets/img/ragazzo.jpg";

export default {
  data() {
    return {
      myElement: null,
      imageUrl: donna,
      image2Url: donna2,
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
</style>
