<template>
  <h1>{{ text }}</h1>
</template>

<script>
export default {
  props: {
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
h1 {
  font-size: 2.25rem;
  font-weight: 600;
  color: #000;
}
</style>
