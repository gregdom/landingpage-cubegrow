<template>
  <div>
    <Header />
    <Hero />
    <Features />
    <Services />
    <Media />
    <SocialProof />
    <Accordion />
    <Footer />
  </div>
</template>

<script>
import {
  Header,
  Hero,
  Features,
  Services,
  Media,
  SocialProof,
  Accordion,
  Footer,
} from '@/components/03-organisms'

export default {
  components: {
    Header,
    Hero,
    Features,
    Services,
    Media,
    SocialProof,
    Accordion,
    Footer,
  },
}
</script>

<style scoped></style>
