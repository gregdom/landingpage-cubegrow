<template>
  <p>{{ text }}</p>
</template>

<script>
export default {
  props: {
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
p {
  font-size: 1.6rem;
  line-height: 30px;
  color: #000;
}
</style>
