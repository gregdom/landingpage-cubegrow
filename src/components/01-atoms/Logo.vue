<template>
  <div class="logo">
    <img class="logo-img" :src="iconPath" alt="Logotipo" />
  </div>
</template>

<script>
export default {
  props: {
    logo: { type: String, required: true },
  },
  computed: {
    iconPath() {
      return require(`@/assets/images/${this.logo}`)
    },
  },
}
</script>

<style scoped>
.logo-img {
  width: 50px;
}
</style>
