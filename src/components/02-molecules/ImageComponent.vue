<template>
  <img :src="imagePath" alt="Image" />
</template>

<script>
export default {
  props: {
    imageName: { type: String, required: true },
  },
  computed: {
    imagePath() {
      return require(`@/assets/images/${this.imageName}`)
    },
  },
}
</script>

<style scoped>
img {
  width: 100%;
}
</style>
