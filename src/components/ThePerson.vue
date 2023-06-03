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
  max-width: 280px;
  height: 20vh;
  border-radius: 25px;
  transition: 0.7s;
}
img:hover {
  transform: scale(1.05);
}
</style>
