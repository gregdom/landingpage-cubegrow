<template>
  <a :href="linkPath">
    {{ linkText }}
  </a>
</template>

<script>
export default {
  props: {
    linkPath: { type: String, required: true },
    linkText: { type: String, required: true },
  },
}
</script>

<style scoped>
a {
  font-weight: 500;
}
</style>
