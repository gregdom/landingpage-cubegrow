<template>
  <nav class="nav">
    <NavItem linkPath="/inicio" linkText="Início" class="active" />
    <NavItem linkPath="/sobre" linkText="Sobre" />
    <NavItem linkPath="/cases" linkText="Cases" />
    <NavItem linkPath="/contato" linkText="Contato" />
  </nav>
</template>

<script>
import { NavItem } from '@/components/01-atoms'

export default {
  components: { NavItem },
}
</script>

<style scoped>
.nav {
  /* margin-bottom: 32px;
  font-size: 20px;
  color: #fff; */
  display: flex;
  flex-direction: column;
}

.nav > * {
  width: 100%;
  margin-bottom: 16px;
  display: block;
  font-size: 20px;
  color: #fff;
}

.nav > *:last-child {
  margin-bottom: 32px;
}

@media screen and (min-width: 768px) {
  .nav {
    all: unset;
    display: flex;
    flex-direction: row;
  }

  .nav > * {
    width: unset;
    margin-right: 16px;
    margin-bottom: 0;
    font-size: 17px;
    color: var(--text-primary-purple-color);
  }

  .nav > *:last-child {
    margin-bottom: 0;
    margin-right: 0;
  }
}
</style>
