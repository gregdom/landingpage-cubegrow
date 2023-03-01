<template>
  <section class="section-features">
    <div class="container">
      <div class="snippet">
        <SnippetSession text="FEATURES" />
      </div>
      <div class="block">
        <SecondTitle
          text="O essencial para administrar suas marcas com eficiência"
        />
        <div class="features-itens">
          <div class="itens">
            <Image imageName="network.svg" />
            <ThirdTitle text="Ampla Variedade" />
            <GeneralText
              text="Produtos e serviços para atender suas necessidades de marketing, desde estratégias de conteúdo até publicidade online."
            />
            <a href="#"
              >Saiba mais
              <span class="material-icons"> arrow_right_alt </span></a
            >
          </div>
          <div class="itens">
            <Image imageName="contract.svg" />
            <ThirdTitle text="Sem Contratos Longos" />
            <GeneralText
              text="Flexibilidade para que você possa escolher os serviços que deseja, sem a obrigação de assinar contratos longos."
            />
            <a href="#"
              >Saiba mais
              <span class="material-icons"> arrow_right_alt </span></a
            >
          </div>
          <div class="itens">
            <Image imageName="money.svg" />
            <ThirdTitle text="Sem Taxas Ocultas" />
            <GeneralText
              text="Valorizamos a transparência e garantimos que não há taxas ocultas em nossos serviços de marketing."
            />
            <a href="#"
              >Saiba mais
              <span class="material-icons"> arrow_right_alt </span></a
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import {
  SnippetSession,
  SecondTitle,
  ThirdTitle,
  GeneralText,
} from '@/components/01-atoms'
import { Image } from '@/components/02-molecules'

export default {
  components: {
    SnippetSession,
    SecondTitle,
    Image,
    ThirdTitle,
    GeneralText,
  },
}
</script>

<style scoped>
.section-features {
  width: 100%;
  height: auto;
}

.section-features .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 64px 0;
}

.section-features .container .snippet-session {
  margin: 0 auto;
}

.section-features .container .block h2 {
  text-align: center;
  padding: 32px 0 40px 0;
}

.section-features .container .block .features-itens > * {
  margin-bottom: 64px;
}
.section-features .container .block .features-itens > *:last-child {
  margin-bottom: 0;
}

.section-features .container .block .features-itens .itens {
  text-align: center;
}

.section-features .container .block .features-itens .itens img {
  width: 60px;
}

.section-features .container .block .features-itens .itens h3 {
  margin: 16px 0 10px 0;
}

.section-features .container .block .features-itens .itens a {
  margin-top: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.6rem;
  color: var(--primary-color);
}

.section-features .container .block .features-itens .itens a > * {
  margin-left: 8px;
}

@media screen and (min-width: 576px) {
  .section-features .container {
    max-width: 70%;
  }
}

@media screen and (min-width: 768px) {
  .section-features .container {
    max-width: 1080px;
    padding: 84px 0 32px 0;
  }

  .section-features .container .block h2 {
    width: 60%;
    margin: 0 auto;
    padding: 32px 0 40px 0;
  }

  .section-features .container .block .features-itens {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }

  .section-features .container .block .features-itens > * {
    margin-right: 22px;
  }

  .section-features .container .block .features-itens > *:last-child {
    margin-right: 0;
    margin-bottom: 64px;
  }

  .section-features .container .block .features-itens h3,
  .section-features .container .block .features-itens p {
    font-size: 25px;
  }
}
</style>
