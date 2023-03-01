<template>
  <i class="fa-brands icon-branding" :class="iconName"></i>
</template>

<script>
export default {
  props: {
    iconName: { type: String, required: true },
  },
}
</script>

<style scoped>
.icon-branding {
  font-size: 48px;
}
</style>
