<template>
  <section class="section-accordion">
    <div class="container">
      <SnippetSession text="FAQ" />
      <SecondTitle text="Você tem perguntas, nós temos respostas" />

      <accordion-item
        v-for="(item, index) in items"
        :key="index"
        :title="item.title"
        :content="item.content"
      ></accordion-item>

      <div class="still-question">
        <Image imageName="faq-people.png" />
        <SecondTitle text="Ainda tem dúvidas?" />
        <GeneralText
          text="Não encontrou a resposta que procura? Converse com nossa equipe."
        />
        <SecondaryButton linkPath="/contato" linkText="info@cubegrow.com" />
      </div>
    </div>
  </section>
</template>

<script>
import {
  AccordionItem,
  SnippetSession,
  SecondTitle,
  GeneralText,
  SecondaryButton,
} from '@/components/01-atoms'
import { Image } from '@/components/02-molecules'

export default {
  components: {
    AccordionItem,
    SnippetSession,
    SecondTitle,
    Image,
    GeneralText,
    SecondaryButton,
  },
  data() {
    return {
      items: [
        {
          title: 'Quais são as áreas de especialização da CubeGrow?',
          content:
            'Nós nos especializamos em marketing de conteúdo, SEO, publicidade online, marketing de mídia social e marketing por e-mail.',
        },
        {
          title:
            'Como vocês planejam aumentar meu tráfego e conversão de vendas?',
          content:
            'Usamos estratégias de marketing personalizadas para aumentar o tráfego, segmentar seu público-alvo e automatizar seu fluxo de trabalho de e-mail.',
        },
        {
          title:
            'Vocês têm experiência em trabalhar com empresas do meu setor?',
          content:
            'Sim, temos experiência em trabalhar com empresas de diversos setores, incluindo o seu.',
        },
        {
          title:
            'Quais são os custos associados aos seus serviços de marketing digital?',
          content:
            'Os custos dos nossos serviços variam de acordo com o tipo de trabalho e a duração da campanha. Oferecemos pacotes personalizados para atender às necessidades do seu negócio.',
        },
        {
          title:
            'Vocês oferecem relatórios de desempenho e análise para monitorar o sucesso da campanha?',
          content:
            'Sim, fornecemos relatórios detalhados sobre o desempenho de sua campanha para que você possa monitorar os resultados e tomar decisões informadas sobre como otimizar sua estratégia de marketing.',
        },
      ],
    }
  },
}
</script>

<style>
.section-accordion {
  width: 100%;
  height: auto;
}

.section-accordion .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 64px 0;
}

.section-accordion .container .snippet-session {
  margin: 0 auto;
}

.section-accordion .container h2 {
  text-align: center;
  padding: 32px 16px;
}

.section-accordion .container .still-question {
  width: 100%;
  height: auto;
  margin: 64px auto 16px auto;
  padding: 64px 16px;
  background: var(--secondary-color);
}

.section-accordion .container .still-question img {
  width: fit-content;
  display: block;
  margin: 0 auto;
}

.section-accordion .container .still-question h2 {
  font-weight: 700;
}

.section-accordion .container .still-question p {
  margin-top: -8px;
  text-align: center;
  color: #878787;
}

.section-accordion .container .still-question .button-secondary {
  width: 85%;
  max-width: 270px;
  margin: 24px auto 0 auto;
  padding: 17px 0;
  font-size: 1.5rem;
}

/* Media Screen min-width 576px */
@media screen and (min-width: 576px) {
  .section-accordion .container {
    width: 70%;
    max-width: 800px;
  }

  .section-accordion .container h2 {
    max-width: 560px;
    text-align: center;
    margin: 0 auto;
    padding: 32px 32px;
  }

  .section-accordion .container .still-question p {
    max-width: 560px;
    margin: -8px auto 0 auto;
    text-align: center;
    color: #878787;
  }
}
</style>
