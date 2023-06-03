<template>
  <button>{{ content }}</button>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: {
    content: {
      type: String,
      required: true,
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
