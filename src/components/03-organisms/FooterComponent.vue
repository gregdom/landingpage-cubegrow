<template>
  <section class="section-footer">
    <div class="container">
      <div class="top">
        <SecondTitle text="Vamos começar algo incrível" />
        <GeneralText
          text="Junte-se a mais de 2.000 startups que estão crescendo com a CubeGrow"
        />
        <PrimaryButton linkPath="/register" linkText="Registre-se agora" />
      </div>

      <div class="base">
        <div class="logoArea">
          <Logo logo="logo-white-color.png" class="logo" />
        </div>

        <div class="copyrightArea">
          <p>Copyright © 2020- 2023 CubeGrow. All Rights Reserved.</p>
        </div>

        <div class="socialArea social">
          <div>
            <a href="/facebook"><IconImages iconName="fa-facebook" /></a>
            <a href="/twitter"><IconImages iconName="fa-twitter" /></a>
            <a href="/instagram"><IconImages iconName="fa-instagram" /></a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import {
  Logo,
  IconImages,
  SecondTitle,
  GeneralText,
  PrimaryButton,
} from '@/components/01-atoms'

export default {
  components: {
    Logo,
    IconImages,
    SecondTitle,
    GeneralText,
    PrimaryButton,
  },
}
</script>

<style scoped>
.section-footer {
  width: 100%;
  height: auto;
  background: var(--third-bg);
}

.section-footer .container {
  width: 90%;
  max-width: 1440px;
  height: auto;
  margin: 0 auto;
  padding: 64px 0 32px 0;
}

.section-footer .container .top {
  width: 100%;
  max-width: 800px;
  margin: 0 auto;
  padding-bottom: 64px;
}

.section-footer .container .top h2 {
  text-align: center;
  color: #fff;
}

.section-footer .container .top p {
  font-size: 1.5rem;
  text-align: center;
  padding: 16px 0 32px 0;
  color: #c4c2c2;
}

.section-footer .container .top .button-primary {
  width: 80%;
  max-width: 270px;
  font-size: 1.5rem;
  margin: 0 auto;
  padding: 15px 0;
}

.section-footer .container .base {
  display: grid;
  grid-template-columns: repeat(2, 50%);
  grid-template-rows: repeat(2, auto);
  grid-template-areas:
    'logoArea socialArea'
    'copyrightArea copyrightArea';
  align-items: center;
  justify-content: space-between;
  padding-top: 64px;
  border-top: 1px solid #fff;
}

.section-footer .container .base .logoArea {
  grid-area: logoArea;
}

.section-footer .container .base .socialArea div {
  grid-area: socialArea;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-end;
}

.section-footer .container .base .socialArea div > * {
  margin-right: 32px;
}

.section-footer .container .base .socialArea div > *:last-child {
  margin-right: 0;
}

.section-footer .container .base .socialArea div a {
  color: #fff;
}

.section-footer .container .base .socialArea div a i {
  font-size: 1.9rem;
}

.section-footer .container .base .copyrightArea {
  grid-area: copyrightArea;
  margin-top: 32px;
}

.section-footer .container .base .copyrightArea p {
  text-align: center;
  line-height: 30px;
  color: #fff;
}

/* 768px */
@media screen and (min-width: 768px) {
  .section-footer .container .base {
    padding-top: 32px;
  }
}

@media screen and (min-width: 992px) {
  .section-footer .container .base {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 32px;
    border-top: 1px solid #fff;
  }

  .section-footer .container .base .logoArea {
    grid-area: unset;
  }

  .section-footer .container .base .socialArea div {
    grid-area: unset;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-end;
  }

  .section-footer .container .base .socialArea div > * {
    margin-right: 16px;
  }

  .section-footer .container .base .socialArea div > *:last-child {
    margin-right: 0;
  }

  .section-footer .container .base .socialArea div a {
    color: #fff;
  }

  .section-footer .container .base .socialArea div a i {
    font-size: 1.9rem;
  }

  .section-footer .container .base .copyrightArea {
    grid-area: unset;
    margin-top: 0;
  }
}
</style>
