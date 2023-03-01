<template>
  <h2>{{ text }}</h2>
</template>

<script>
export default {
  props: {
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
h2 {
  font-size: 2.25rem;
  font-weight: 600;
  line-height: 40px;
  color: #000;
}
</style>
