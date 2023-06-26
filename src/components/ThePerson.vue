<template>
  <div>
    <figure class="flex flex-col justify-center mb-10">
      <img :src="img" :alt="name" />
      <figcaption>
        <h3 class="mt-4 mb-1">{{ name }}</h3>
        <h4>{{ job }}</h4>
      </figcaption>
    </figure>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    img: {
      type: String,
      required: true,
    },
    job: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
div {
  width: 280px;
}
h3 {
  max-width: 280px;
  text-align: center;
  color: var(--rosa);
  font-family: "SF Bold";
  font-size: 1.4rem;
}
h4 {
  max-width: 280px;
  text-align: center;
}
img {
  background-size: cover;
  min-width: 230px;
  max-width: 280px;
  height: 20vh;
  border-radius: 25px;
  transition: 0.7s;
  box-shadow: rgba(255, 255, 255, 0.1) 0px 1px 1px 0px inset,
    rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
}
img:hover {
  transform: scale(1.05);
}
@media (max-width: 430px) {
  img {
    margin-left: -3.8rem !important;
  }
  h3,
  h4 {
    margin-left: -30px;
  }
}
</style>
