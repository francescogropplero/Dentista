<template>
  <a :href="link">
    <button>{{ content }}</button>
  </a>
</template>

<script>
export default {
  props: {
    content: {
      type: String,
      required: true,
    },
    link: {
      type: String,
      required: false,
    },
  },
};
</script>

<style scoped>
button {
  align-items: center;
  padding: 0.5em;
  padding-left: 3rem;
  padding-right: 3rem;
  border-radius: 25px;
  font-family: "SF Semibold";
  font-size: large;
  background-color: var(--rosa);
  transition: 0.5s;
  color: white;
  margin: 0 auto !important;
  text-align: center;
}
</style>
