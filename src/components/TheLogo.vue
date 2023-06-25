<template>
  <div class="padre">
    <a href="#">
      <img src="../assets/img/logoDentista.png" alt="Dentist Logo" />
    </a>
  </div>
</template>

<style scoped>
.padre {
  height: 9vh;
  width: 15vw;
}
img {
  height: 100%;
  min-width: 90px;
}
@media (max-width: 430px) {
  .padre {
    margin-left: -1.5rem;
    height: 15vh;
    width: 35vw;
  }
}
</style>
