<template>
  <div>
    <figure class="flex flex-col justify-center mt-28 mb-10">
      <img :src="img" :alt="name" />
      <figcaption>
        <h3 class="mt-4 mb-1">{{ name }}</h3>
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
  },
};
</script>

<style scoped>
div {
  width: 330px;
}
h3 {
  max-width: 330px;
  text-align: center;
  font-family: "SF Bold";
  font-size: 1.4rem;
}
img {
  background-size: cover;
  min-width: 230px;
  max-width: 330px;
  height: 20vh;
  border-radius: 25px;
  transition: 0.7s;
}
img:hover {
  transform: scale(1.05);
}
@media (max-width: 430px) {
  img {
    margin-left: -3.8rem !important;
  }
  h3 {
    margin-left: -30px;
  }
}
</style>
