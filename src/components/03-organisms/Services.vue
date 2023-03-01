<template>
  <section class="section-services">
    <div class="container">
      <main>
        <div class="blocks-group">
          <div class="block-one blocks">
            <div class="image">
              <Image imageName="optimization.jpg" />
            </div>
            <div class="presentation">
              <SnippetPreContent text="01 - EMAIL MARKETING" />
              <SecondTitle text="Aumente sua receita com Email Marketing" />
              <GeneralText
                text="Relatórios detalhados para monitorar o desempenho de suas campanhas. Aproveite nosso conhecimento em marketing por email para impulsionar suas vendas e aumentar sua receita."
              />
              <PrimaryButton
                linkPath="/registrar"
                linkText="Cresça sua marca agora"
              />
            </div>
          </div>
          <div class="block-two blocks">
            <div class="image">
              <Image imageName="sales.jpg" />
            </div>
            <div class="presentation">
              <SnippetPreContent text="02 - AUMENTO DAS VENDAS" />
              <SecondTitle text="Aumente as vendas em 110%" />
              <GeneralText
                text="Usando estratégias de marketing eficazes, como personalização, segmentação e automação, podemos ajudar sua marca a alcançar novos níveis de crescimento e sucesso."
              />
              <div class="buttons">
                <PrimaryButton linkPath="/contato" linkText="Fale Conosco" />
                <ThirdButton linkPath="/testemunhos" linkText="Nossos Cases" />
              </div>
            </div>
          </div>
        </div>
      </main>
    </div>
  </section>
</template>

<script>
import {
  SnippetPreContent,
  SecondTitle,
  GeneralText,
  PrimaryButton,
  ThirdButton,
} from '@/components/01-atoms'
import { Image } from '@/components/02-molecules'

export default {
  components: {
    SnippetPreContent,
    SecondTitle,
    GeneralText,
    PrimaryButton,
    ThirdButton,
    Image,
  },
}
</script>

<style scoped>
.section-services {
  width: 100%;
  height: auto;
}

.section-services .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 32px 0;
}

.section-services .container .blocks-group {
  display: grid;
}

.section-services .container .blocks-group > * {
  margin-bottom: 64px;
}

.section-services .container .blocks-group > *:last-child {
  margin-bottom: 0;
}

.section-services .container .blocks-group .blocks .snippet-decoration {
  margin-bottom: 16px;
  font-size: 17px;
  padding: 14px 25px 10px 25px;
  margin: 16px auto;
}

.section-services .container .blocks-group .blocks h2 {
  padding: 8px 0 16px 0;
}

.section-services .container .blocks-group .blocks p {
  padding: 16px 0;
}

.section-services .container .blocks-group .blocks .buttons {
  display: flex;
}

.section-services .container .blocks-group .blocks .buttons > * {
  margin-right: 16px;
}

.section-services .container .blocks-group .blocks .buttons > *:last-child {
  margin-right: 0;
}

.section-services .container .blocks-group .blocks .button-primary,
.section-services .container .blocks-group .blocks .button-third {
  padding: 15px 0;
  font-size: 1.4rem;
}

.section-services .container .blocks-group .block-one .button-primary {
  width: 100%;
}

.section-services .container .blocks-group .block-two .button-primary,
.section-services .container .blocks-group .block-two .button-third {
  width: 50%;
}

.section-services .container .blocks-group .block-two .button-primary {
  padding: 17px 0 14px 0;
}

@media screen and (min-width: 576px) {
  .section-services .container {
    max-width: 70%;
  }

  .section-services .container .blocks-group .blocks .image img {
    max-width: 340px;
    display: block;
    margin: 0 auto;
  }
}

@media screen and (min-width: 768px) {
  .section-services .container {
    max-width: 1080px;
    padding-bottom: 84px;
  }

  .section-services .container .blocks-group .blocks .snippet-decoration {
    margin: 16px 0;
  }

  .section-services .container .blocks-group .blocks {
    display: grid;
    grid-template-columns: repeat(2, 50%);
    align-items: center;
    justify-content: space-between;
  }

  /* Position change */
  .section-services .container .blocks-group .block-one {
    display: grid;
    grid-template-columns: repeat(2, 50%);
    grid-template-areas: 'image presentation';
  }

  .section-services .container .blocks-group .block-one .image {
    grid-area: presentation;
  }

  .section-services .container .blocks-group .block-one .presentation {
    grid-area: image;
  }
  /* ******* */

  .section-services .container .blocks-group .blocks .image img {
    max-width: 100%;
    display: block;
    margin: 0 auto;
  }

  .section-services .container .blocks-group .block-one .presentation {
    padding: 0 32px 0 0;
  }

  .section-services .container .blocks-group .block-one .button-primary {
    width: max-content;
    padding-left: 25px;
    padding-right: 25px;
  }

  .section-services .container .blocks-group .block-two .presentation {
    padding: 0 0 0 32px;
  }
}
</style>
