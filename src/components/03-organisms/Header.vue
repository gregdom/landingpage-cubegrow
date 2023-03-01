<template>
  <header class="header">
    <!-- Desktop -->
    <div class="container-desktop">
      <div class="menu-desktop">
        <Logo logo="logo-main-color.png" />
        <div class="pos-right">
          <div>
            <NavBar />
          </div>

          <div class="buttons">
            <PrimaryButton linkPath="/start" linkText="Registre-se" />
            <SecondaryButton linkPath="/login" linkText="Login" />
          </div>
        </div>
      </div>

      <!-- Mobile -->
      <div class="container-mobile">
        <Logo logo="logo-main-color.png" />
        <span class="material-icons open-icon" @click="toggleMenu"> menu </span>
        <div class="menu-mobile" :class="{ open: isOpen }">
          <div class="top">
            <span class="material-icons close-icon" @click="toggleMenu">
              close
            </span>
            <Logo logo="logo-white-color.png" />
          </div>
          <div class="pos-right">
            <div>
              <NavBar />
            </div>

            <div class="buttons">
              <PrimaryButton linkPath="/start" linkText="Registre-se" />
              <SecondaryButton linkPath="/login" linkText="Login" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import { Logo, PrimaryButton, SecondaryButton } from '@/components/01-atoms'
import { NavBar } from '@/components/02-molecules'

export default {
  components: { Logo, PrimaryButton, SecondaryButton, NavBar },
  data() {
    return {
      isOpen: false,
    }
  },
  methods: {
    toggleMenu() {
      console.log('teste')
      console.log(this.isOpen)
      this.isOpen = !this.isOpen
    },
  },
}
</script>

<style scoped>
.header {
  width: 100%;
  height: 100px;
  font-family: 'Poppins', sans-serif;
  border-bottom: 1px solid #d7dbfc88;
  background: var(--primary-bg);
}

.header .container-desktop .menu-desktop,
.header .container-mobile .menu-mobile {
  max-width: 1440px;
}

.header .container-desktop .menu-desktop {
  display: none;
}

.header .container-mobile {
  width: 100%;
  height: 100px;
  margin: 0 auto;
  position: relative;
}

.header .container-mobile .open-icon,
.header .container-mobile .menu-mobile .top .close-icon {
  padding: 5px 5px 5px 0;
  font-size: 32px;
  cursor: pointer;
  color: var(--text-primary-purple-color);
}

.header .container-mobile .logo {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.header .container-mobile .open-icon {
  position: absolute;
  top: 50%;
  left: 14px;
  transform: translateY(-50%);
}

/* Menu */
.header .container-mobile .menu-mobile {
  width: 100%;
  max-width: 250px;
  height: 100%;
  padding: 0 16px;
  position: fixed;
  top: 0;
  left: -250px;
  transition: all 0.3s ease-in-out;
  background: var(--primary-color);
}

.header .container-mobile .menu-mobile.open {
  left: 0;
  transition: all 0.3s ease-in-out;
}

.header .container-mobile .menu-mobile .top {
  width: 100%;
  height: 100px;
  margin-bottom: 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid #d7dbfc88;
}

.header .container-mobile .menu-mobile .top .close-icon {
  color: #fff;
}

.header .container-mobile .menu-mobile .top .logo {
  all: unset;
}

.header .container-mobile .menu-mobile .pos-right .buttons a {
  width: 100%;
  margin-bottom: 16px;
  padding: 10px 0;
}

.header .container-mobile .menu-mobile .pos-right .buttons a.button-primary {
  font-size: 18px;
  background: #fff;
  color: var(--primary-color);
}

.header .container-mobile .menu-mobile .pos-right .buttons a.button-secondary {
  font-size: 18px;
  color: #fff;
  border: 1px solid #fff;
}

@media screen and (min-width: 768px) {
  /* Disable */
  .header .container-desktop .container-mobile,
  .header .container-desktop .menu-mobile,
  .header .container-mobile .open-icon,
  .header .container-mobile .logo {
    display: none;
  }
  /*****/

  .header .container-desktop .menu-desktop {
    width: 90%;
    height: 100px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(2, auto);
    align-items: center;
    justify-content: space-between;
  }

  .header .container-desktop .menu-desktop .pos-right {
    display: flex;
    align-items: center;
  }

  .header .container-desktop .menu-desktop .pos-right > * {
    margin-right: 32px;
  }
  .header .container-desktop .menu-desktop .pos-right > *:last-child {
    margin-right: 0;
  }

  .header .container-desktop .menu-desktop .pos-right .buttons {
    display: flex;
    align-items: center;
  }

  .header .container-desktop .menu-desktop .pos-right .buttons > * {
    font-size: 16px;
    margin-right: 16px;
  }

  .header .container-desktop .menu-desktop .pos-right .buttons > *:last-child {
    margin-right: 0;
  }

  .header
    .container-desktop
    .menu-desktop
    .pos-right
    .buttons
    a.button-primary {
    font-size: 16px;
  }

  .header
    .container-desktop
    .menu-desktop
    .pos-right
    .buttons
    a.button-secondary {
    font-size: 16px;
  }
}
</style>
