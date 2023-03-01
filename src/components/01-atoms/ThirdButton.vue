<template>
  <a :href="linkPath" class="button-third">
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
.button-third {
  width: 125px;
  padding: 7px 0;
  display: block;
  font-size: 16px;
  text-align: center;
  color: var(--text-black-color);
  border-radius: 5px;
  border: var(--border);
  background: transparent;
}
</style>
