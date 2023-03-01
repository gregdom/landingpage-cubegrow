<template>
  <a :href="linkPath" class="button-secondary">
    {{ linkText }}
  </a>
</template>

<script>
export default {
  props: {
    linkPath: { type: String, required: true },
    linkText: { type: String, required: true },
  },
  computed: {},
}
</script>

<style scoped>
.button-secondary {
  width: 125px;
  padding: 7px 0;
  display: block;
  font-size: 16px;
  text-align: center;
  color: var(--primary-color);
  border-radius: 5px;
  background-color: var(--secondary-color);
}
</style>
