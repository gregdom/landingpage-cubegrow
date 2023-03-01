<template>
  <div class="snippet-session">
    <span> {{ text }} </span>
  </div>
</template>

<script>
export default {
  props: {
    text: { type: String, required: true },
  },
}
</script>

<style scoped>
.snippet-session {
  width: fit-content;
  padding: 11px 25px 6px 25px;
  border-radius: 6px;
  color: var(--primary-color);
  background: var(--secondary-color);
}

.snippet-session span {
  font-weight: 600;
}
</style>
