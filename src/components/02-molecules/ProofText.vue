<template>
  <div class="text-group">
    <GeneralText text="01" class="rank" />

    <GeneralText
      text="In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content. Lorem ipsum."
      class="description"
    />

    <div>
      <GeneralText text="50%" class="percentage" />
      <GeneralText text="Sales performance increased" class="support" />
    </div>
  </div>
</template>

<script>
import { GeneralText } from '@/components/01-atoms'

export default {
  components: {
    GeneralText,
  },
}
</script>

<style scoped>
.text-group {
  margin: 16px 0 0 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.section-proof .text-group .rank {
  text-align: center;
  font-size: 14.5rem;
  line-height: 10rem;
  color: #fff;
}

.section-proof .text-group .description {
  width: 100%;
  height: auto;
  padding-bottom: 32px;
  text-align: center;
  color: #fff;
  border-bottom: 1px solid #313b46;
}

.section-proof .text-group .percentage {
  width: 100%;
  margin-top: 32px;
  text-align: center;
  font-size: 5rem;
  font-weight: 600;
  line-height: 5rem;
  color: #fff;
}

.section-proof .text-group .support {
  font-size: 1.4rem;
  text-align: center;
  color: #ffffff66;
}
</style>
