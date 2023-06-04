<template>
  <TheNavbar />
  <TheHero />
  <div class="flex flex-wrap">
    <FirstDescription />
    <ThePeople />
  </div>
  <SecondDescription />
</template>

<script setup>
import TheNavbar from "./components/TheNavbar.vue";
import TheHero from "./components/TheHero.vue";
import FirstDescription from "./components/FirstDescription.vue";
import SecondDescription from "./components/SecondDescription.vue";
import ThePeople from "./components/ThePeople.vue";
</script>
