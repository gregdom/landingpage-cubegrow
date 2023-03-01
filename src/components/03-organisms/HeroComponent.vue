<template>
  <section class="section-hero">
    <div class="container">
      <div class="first-block">
        <SnippetPreContent emoji="🙋‍♀️" text="Olá, somos a CubeGrow!" />
        <HeroText />

        <div class="buttons">
          <PrimaryButton linkPath="/start" linkText="Registre-se" />
          <ThirdButton linkPath="/learn" linkText="Saiba Mais" />
        </div>
      </div>
      <div class="second-block">
        <Image imageName="dashboard.png" />
      </div>
    </div>

    <div class="icons-block">
      <div>
        <p>Confiança de centenas de marcas no mundo</p>
      </div>
      <div class="icons-group">
        <IconImages iconName="fa-digg" />
        <IconImages iconName="fa-angular" />
        <IconImages iconName="fa-python" />
        <IconImages iconName="fa-google-drive" />
        <IconImages iconName="fa-github" />
        <IconImages iconName="fa-sass" />
        <IconImages iconName="fa-aws" />
      </div>
    </div>
  </section>
</template>

<script>
import {
  SnippetPreContent,
  PrimaryButton,
  ThirdButton,
  IconImages,
} from '@/components/01-atoms'
import { HeroText, Image } from '@/components/02-molecules'

export default {
  components: {
    SnippetPreContent,
    HeroText,
    Image,
    PrimaryButton,
    ThirdButton,
    IconImages,
  },
}
</script>

<style scoped>
.section-hero {
  width: 100%;
  height: auto;
  background: var(--primary-bg);
}

.section-hero .container {
  width: 90%;
  height: auto;
  margin: 0 auto;
  padding: 32px 0;
}

.section-hero .container .first-block .snippet-decoration {
  margin-bottom: 16px;
  font-size: 17px;
}

.section-hero .container .first-block .buttons {
  margin-top: 16px;
  display: flex;
  flex-direction: column;
}

.section-hero .container .first-block .buttons > * {
  margin-bottom: 16px;
}

.section-hero .container .first-block .buttons > *:last-child {
  margin-bottom: 0;
}

.section-hero .container .first-block .buttons .button-primary,
.section-hero .container .first-block .buttons .button-third {
  width: 100%;
  padding: 15px 0;
  font-size: 1.4rem;
}

.section-hero .icons-block {
  display: none;
}

@media screen and (min-width: 576px) {
  .section-hero .container {
    max-width: 70%;
  }

  .section-hero .container .first-block .buttons {
    margin-top: 32px;
    display: flex;
    flex-direction: row;
  }

  .section-hero .container .first-block .buttons > * {
    margin-right: 16px;
    margin-bottom: 0;
  }

  .section-hero .container .first-block .buttons > *:last-child {
    margin-right: 0;
  }

  .section-hero .container .first-block .buttons .button-primary,
  .section-hero .container .first-block .buttons .button-third {
    width: 100%;
    padding: 12px 0 10px 0;
    font-size: 20px;
  }
}

@media screen and (min-width: 768px) {
  .section-hero .container {
    max-width: 1080px;
    display: grid;
    grid-template-columns: repeat(2, 50%);
    align-items: center;
    justify-content: space-between;
  }

  .section-hero .container .first-block {
    padding: 0 32px 0 0;
  }

  .section-hero .container .first-block .snippet-decoration {
    padding: 7px 25px;
  }

  .section-hero .container .first-block .buttons .button-primary,
  .section-hero .container .first-block .buttons .button-third {
    width: 100%;
    max-width: 180px;
    padding: 12px 0 10px 0;
    font-size: 20px;
  }

  .section-hero .container .second-block img {
    max-width: 500px;
    display: block;
    float: right;
  }

  .section-hero .icons-block {
    width: 100%;
    height: auto;
    padding: 32px 0 32px 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: var(--primary-bg);
  }

  .section-hero .icons-block p {
    text-align: center;
    margin-bottom: 32px;
    color: var(--text-primary-purple-color);
  }

  .section-hero .icons-block .icons-group {
    max-width: 1080px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .section-hero .icons-block .icons-group > * {
    margin-right: 42px;
  }

  .section-hero .icons-block .icons-group > *:last-child {
    margin-right: 0;
  }
}
</style>
