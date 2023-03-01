<template>
  <div class="accordion-item">
    <div class="accordion-title" @click="isOpen = !isOpen">
      <div>
        <ThirdTitle :text="title" />
      </div>
      <div>
        <span class="material-icons" v-if="!isOpen"> add_circle_outline </span>
        <span class="material-icons" v-else> remove_circle_outline </span>
      </div>
    </div>
    <div class="accordion-content" v-if="isOpen">
      <GeneralText :text="content" />
    </div>
  </div>
</template>

<script>
import { ThirdTitle, GeneralText } from '@/components/01-atoms'

export default {
  props: {
    title: String,
    content: String,
  },
  components: {
    ThirdTitle,
    GeneralText,
  },
  data() {
    return {
      isOpen: false,
    }
  },
}
</script>

<style>
/* .accordion-item {
  border-bottom: 1px solid #dbdbdb;
} */

.accordion-title {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 0 16px 0;
  line-height: 30px;
  cursor: pointer;
}

.accordion-content {
  padding: 0 16px 16px 16px;
}

.accordion-content p {
  color: #878787;
}
</style>
