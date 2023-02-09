<script setup>
import { RouterLink, RouterView } from "vue-router";
import logo from "./assets/images/logo.svg";
import logoSm from "./assets/images/logo-sm.svg";
import shopping from "./assets/images/shopping.svg";
import footerVue from "./components/footerVue.vue";
</script>

<template>
  <header class="header d-flex justify-content-between align-items-center p-2">
    <input type="checkbox" name="nav-toggler" id="nav-toggler" />
    <nav class="nav">
      <RouterLink to="/" class="navList">首頁</RouterLink>
      <RouterLink to="/about" class="navList">最新消息</RouterLink>
      <a href="#" class="navList">美味菜單</a>
      <a href="#" class="navList text-primary">後台登入</a>
    </nav>
    <label for="nav-toggler" class="hamburgerBtn">
      <span class="hamburgerLine"></span>
      <span class="hamburgerLine"></span>
      <span class="hamburgerLine"></span>
    </label>
    <h1 class="headerName">橘 Tachibana</h1>
    <RouterLink to="/">
      <a href="#">
        <img :src="logo" alt="橘 Tachibana" class="logoImg d-none d-md-block" />
        <img
          :src="logoSm"
          alt="橘 Tachibana"
          class="logoImg d-block d-md-none"
        />
      </a>
    </RouterLink>
    <div class="shoppingBtn">
      <img :src="shopping" alt="購物車" class="shoppingCar" />
    </div>
  </header>
  <RouterView />
  <footerVue></footerVue>
</template>

<style scoped lang="scss">
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 5;
  background-color: #1b1b1b;
  &Name {
    display: none;
  }
  #nav-toggler {
    display: none;
  }
  #nav-toggler:checked ~ .nav {
    left: 0;
  }
  #nav-toggler:checked ~ .hamburgerBtn .hamburgerLine:nth-child(1) {
    transform: rotate(45deg);
    transition: bottom 0.5s, transform 0.5s 0.5s;
    background-color: #f25c05;
  }
  #nav-toggler:checked ~ .hamburgerBtn .hamburgerLine:nth-child(2) {
    opacity: 0;
    transition: 0.5s;
  }
  #nav-toggler:checked ~ .hamburgerBtn .hamburgerLine:nth-child(3) {
    transform: rotate(-45deg);
    transition: top 0.5s, transform 0.5s 0.5s;
    background-color: #f25c05;
  }
  .nav {
    position: fixed;
    top: 0;
    left: -110%;
    height: 100%;
    width: 100%;

    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #1b1b1b;
    transition: 1s left;
    .navList {
      font-size: 32px;
      font-weight: 700;
      writing-mode: vertical-rl;
      padding: 16px;
      letter-spacing: 12px;
      @media (max-width: 768px) {
        font-size: 24px;
      }
    }
    @media (max-width: 768px) {
      font-size: 24px;
      padding: 8px;
    }
  }
  .hamburgerBtn,
  .shoppingBtn {
    height: 80px;
    width: 80px;
    cursor: pointer;

    padding: 24px;
    @media (max-width: 768px) {
      width: 48px;
      height: 48px;
      padding: 8px;
    }
  }
  .hamburgerBtn {
    position: relative;
  }
  .hamburgerLine {
    width: 32px;
    height: 4px;
    background-color: #fff;
    border-radius: 4px;
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    margin: auto;
    &:nth-child(1) {
      transform: translateY(-12px);
      transition: bottom 0.5s 0.5s, transform 0.5s;
    }
    &:nth-child(2) {
      top: 0;
      bottom: 0;
      transition: 0.5s 0.5s;
    }
    &:nth-child(3) {
      transform: translateY(12px);
      transition: top 0.5s 0.5s, transform 0.5s;
    }
  }
}
</style>
