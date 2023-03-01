<template>
  <div class="snippet-decoration">
    {{ emoji }} <span> {{ text }} </span>
  </div>
</template>

<script>
export default {
  props: {
    emoji: { type: String, required: false },
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
.snippet-decoration {
  width: fit-content;
  padding: 10px 25px;
  white-space: nowrap;
  border-top-left-radius: 12px;
  border-top-right-radius: 12px;
  border-bottom-right-radius: 12px;
  color: var(--primary-color);
  background: var(--secondary-color);
}

.snippet-decoration span {
  font-weight: 600;
}
</style>
