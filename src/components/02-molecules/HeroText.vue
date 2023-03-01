<template>
  <div>
    <PrimaryTitle text="Ajudamos marcas de e-commerce a crescer" />
    <GeneralText
      text="Soluções de marketing digital personalizadas para aumentar o tráfego, a conversão e a retenção de clientes, impulsionando o sucesso de sua marca."
    />
  </div>
</template>

<script>
import { PrimaryTitle, GeneralText } from '@/components/01-atoms'

export default {
  components: { PrimaryTitle, GeneralText },
}
</script>

<style scoped>
h1 {
  margin-bottom: 16px;
  line-height: 45px;
}

p {
  line-height: 30px;
}

@media screen and (min-width: 768px) {
  h1 {
    font-size: 40px;
    line-height: 45px;
  }

  p {
    font-size: 25px;
    line-height: 30px;
  }
}
</style>
