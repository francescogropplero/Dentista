<template>
  <TheNavbar />
  <TheHero />
  <div class="flex flex-wrap">
    <FirstDescription />
    <ThePeople />
  </div>
  <SecondDescription />
  <GroupInsurance />
  <TheForm />
  <TheFooter />
</template>

<script setup>
import TheNavbar from "./components/TheNavbar.vue";
import TheHero from "./components/TheHero.vue";
import FirstDescription from "./components/FirstDescription.vue";
import SecondDescription from "./components/SecondDescription.vue";
import ThePeople from "./components/ThePeople.vue";
import GroupInsurance from "./components/GroupInsurance.vue";
import TheForm from "./components/TheForm.vue";
import TheFooter from "./components/TheFooter.vue";
</script>
