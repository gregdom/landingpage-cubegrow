<template>
  <section class="section-media">
    <div class="container">
      <SnippetSession text="ESTAMOS NA MÍDIA" />
      <SecondTitle
        text="“A melhor equipe para ajudá-lo a crescer. Simples assim.”"
      />
      <GeneralText text="Amado por centenas de marcas no ramo B2C" />

      <div class="images">
        <Image imageName="glossom-logo.png" />
        <Image imageName="animal-logo.png" />
      </div>

      <PrimaryButton linkPath="/contato" linkText="+1 386 597 92877" />

      <GeneralText text="Agende uma ligação" class="support" />
    </div>
  </section>
</template>

<script>
import {
  SnippetSession,
  SecondTitle,
  GeneralText,
  PrimaryButton,
} from '@/components/01-atoms'
import { Image } from '@/components/02-molecules'

export default {
  components: {
    SnippetSession,
    SecondTitle,
    GeneralText,
    Image,
    PrimaryButton,
  },
}
</script>

<style scoped>
.section-media {
  width: 100%;
  height: auto;
  margin: 32px 0 0 0;
  background: var(--secondary-bg);
}

.section-media .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 64px 0;
}

.section-media .container .snippet-session {
  width: 60%;
  max-width: 270px;
  margin: 0 auto;
  text-align: center;
  padding: 11px 25px 6px 25px;
}

.section-media .container h2 {
  margin: 32px 0 16px 0;
  text-align: center;
}

.section-media .container p {
  text-align: center;
  color: var(--text-secondary-purple-color);
}

.section-media .container .images {
  margin: 32px auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.section-media .container .images > * {
  margin-bottom: 16px;
}

.section-media .container .images > *:last-child {
  margin-bottom: 0;
}

.section-media .container .images img {
  width: 100%;
  max-width: 168px;
}

.section-media .container .button-primary {
  width: 100%;
  max-width: 270px;
  padding: 17px 30px 15px 30px;
  margin: 0 auto 10px auto;
  font-size: 1.4rem;
}

.section-media .container .support {
  font-size: 1.4rem;
  color: #000;
}

/* Media Screen min-width 576px */
@media screen and (min-width: 576px) {
  .section-media .container {
    width: 70%;
    max-width: 535px;
  }
}

/* Media Screen min-width 768px */
@media screen and (min-width: 768px) {
  .section-media .container .images {
    margin: 32px auto;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }

  .section-media .container .images > * {
    margin-right: 16px;
    margin-bottom: 0;
  }
}
</style>
