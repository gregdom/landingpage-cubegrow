<template>
  <h3>{{ text }}</h3>
</template>

<script>
export default {
  props: {
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
h3 {
  font-size: 1.6rem;
  font-weight: 600;
  color: #000;
}
</style>
