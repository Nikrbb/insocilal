<template>
  <div class="container">
      <header class="header">
        <div class="header__logo">
          <img class="header__logo-image" src="../assets/logo.png" alt="logo">
        </div>
        <div class="header__menu">
          <ul class="header__list">
            <li class="header__list-item">
              <a class="header__submenu"  :class="{ 'header__submenu--active': isActiveHeaderMenu }"  @click="toggle" href="#">Products
                <span class="header__toggle"  :class="{ 'header__toggle--active': isActiveHeaderMenu }"></span>
              </a>
            </li>
            <li class="header__list-item"><a href="#">Why INSOCIAL?</a></li>
            <li class="header__list-item"><a href="#">Pricing</a></li>
            <li class="header__list-item"><a href="#">About</a></li>
            <li class="header__list-item"><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="header__sign-section">
          <a href="#" class="header__sign-in">SIGN IN</a>
          <main-button></main-button>
        </div>
    </header>
  </div>

</template>

<script>
import MainButton from './MainButton'

export default {
  name: 'Header',
  components: {
    MainButton
  },
  data() {
    return {
      isActiveHeaderMenu: false,
    }
  },
  methods: {
    toggle() {
      this.isActiveHeaderMenu = !this.isActiveHeaderMenu;
    }
  }


}
</script>

<style lang="scss" scoped>
.container {
  padding: 13px 0;
}
.header {
  display: flex;

  &__logo {}
  &__logo-image {
    max-width: 250px;
  }
  &__menu {
    display: flex;
    align-items: center;
  }
  &__list {
    display: flex;
    align-items: center;
    gap: 32px;
    padding: 0;
    margin: 0 0 0 50px;
    white-space: nowrap;
  }
  &__list-item {
  display: flex;
  }

  &__submenu {
    padding: 16px 8px;
    transition: 0.5s;
  }

  &__submenu--active {
    background: #F8F8F8;
    border-radius: 8px;
  }

  &__toggle {
    display: inline-block;
    margin-left: 17px;
    width: 9px;
    height: 9px;
    border-right: 2px solid black;
    border-bottom: 2px solid black;
    border-radius: 2px;
    background: none;
    transform: rotateZ(45deg);
    transition: inherit;
  }

  &__toggle--active {
    transform: rotateZ(-135deg)
  }

  &__sign-section {
    display: flex;
    align-items: center;
    white-space: nowrap;
  }
  &__sign-in {
    margin: 0 16px 0 56px;
    font-weight: 700;
  }


}
</style>