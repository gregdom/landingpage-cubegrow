<template>
  <section class="section-proof">
    <div class="container">
      <SnippetSession text="CONFIABILIDADE" />
      <SecondTitle
        text="Marcas icônicas que aumentaram seu desempenho de vendas"
      />

      <div class="wrapper">
        <div class="text-group block-one">
          <GeneralText text="01" class="rank" />

          <GeneralText
            text="“Com a ajuda da equipe de marketing digital, pude aumentar meu tráfego em mais de 50% e dobrar minhas vendas em menos de seis meses. 
            Agora minha marca é um nome icônico nessa indústria.”"
            class="description"
          />

          <div>
            <GeneralText text="50%" class="percentage" />
            <GeneralText text="de desempenho" class="support" />
          </div>
        </div>

        <div class="text-group block-two">
          <GeneralText text="02" class="rank" />

          <GeneralText
            text="“A CubeGrow foi fundamental para o sucesso do meu negócio. Eles criaram uma estratégia de marketing personalizada para minha marca de e-commerce, o que resultou em um aumento de 60% nas vendas.”"
            class="description"
          />

          <div>
            <GeneralText text="60%" class="percentage" />
            <GeneralText text="de desempenho" class="support" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { SnippetSession, SecondTitle, GeneralText } from '@/components/01-atoms'

export default {
  components: {
    SnippetSession,
    SecondTitle,
    GeneralText,
  },
}
</script>

<style scoped>
.section-proof {
  width: 100%;
  height: auto;
  background: var(--third-bg);
}

.section-proof .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 64px 0;
}

.section-proof .container .snippet-session {
  width: 70%;
  max-width: 270px;
  margin: 0 auto;
  text-align: center;
  padding: 11px 25px 6px 25px;
  color: #fff;
  background: #313b46;
}

.section-proof .container h2 {
  padding: 35px 0 70px 0;
  text-align: center;
  font-weight: 600;
  color: #fff;
}

.section-proof .container .text-group {
  margin: 16px 0 0 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.section-proof .container .block-one {
  padding-bottom: 64px;
  border-bottom: 1px solid #313b46;
}

.section-proof .container .block-two {
  padding-top: 68px;
}

.section-proof .container .text-group .rank {
  text-align: center;
  font-size: 14.5rem;
  line-height: 10rem;
  color: #fff;
}

.section-proof .container .text-group .description {
  width: 100%;
  height: auto;
  padding: 10px 0 32px 0;
  text-align: center;
  color: #fff;
}

.section-proof .container .text-group .percentage {
  width: 100%;
  margin-top: 32px;
  text-align: center;
  font-size: 5rem;
  line-height: 5rem;
  color: #fff;
}

.section-proof .container .text-group .support {
  font-size: 1.4rem;
  text-align: center;
  color: #c4c2c2;
}

/* Media Screen min-width 576px */
@media screen and (min-width: 576px) {
  .section-proof .container {
    width: 70%;
    max-width: 535px;
  }
}

/* Media Screen min-width 992px */
@media screen and (min-width: 992px) {
  .section-proof .container {
    width: 100%;
    max-width: 800px;
    margin: 0 auto;
    padding-bottom: 94px;
  }

  .section-proof .container h2 {
    width: 560px;
    margin: 0 auto;
    padding: 35px 0 70px 0;
  }

  .section-proof .container .text-group {
    margin: 16px 0 0 0;
    display: grid;
    grid-template-columns: 140px auto 200px;
    align-items: center;
    justify-content: center;
  }

  .section-proof .container .text-group .rank {
    text-align: left;
    font-size: 10rem;
    line-height: 5rem;
  }

  .section-proof .container .text-group .description {
    text-align: left;
    padding: 0 0 0 64px;
  }

  .section-proof .container .text-group .percentage {
    margin-top: 0;
    text-align: center;
  }
}
</style>
