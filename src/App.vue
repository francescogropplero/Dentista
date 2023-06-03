<template>
  <TheNavbar />
  <TheHero />
  <div class="flex">
    <FirstDescription />
    <ThePeople />
  </div>
</template>

<script setup>
import TheNavbar from "./components/TheNavbar.vue";
import TheHero from "./components/TheHero.vue";
import FirstDescription from "./components/FirstDescription.vue";
import ThePeople from "./components/ThePeople.vue";
</script>
