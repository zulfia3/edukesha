<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
  <header class="header">
    <nav class="navigation">
      <div class="container">
        <div class="navigation__wrap">
          <img src="/logo.svg" alt="" />
          <div :class="['navigation__menu', { 'open': isMenuOpen }]">
            <ul class="navigation__menu-list">
              <li class="navigation__menu-item">
                <a href="" class="navigation__menu-link"> Возможности </a>
              </li>
              <li class="navigation__menu-item">
                <a href="" class="navigation__menu-link"> Как это работает? </a>
              </li>
            </ul>
              <div class="navigation__menu-info">
              <p>г Сургут, ул Базовая, д. 34, офис 10 <br />
                ОГРН 1238600001200 <br />
                ИНН 8602309464 </p>
                <p>ООО Дотсолюшн © 2023</p>
              </div>
          </div>
          <div class="navigation__list">
            <ul class="navigation__list-link">
              <li class="navigation__list-link-item">
                <a href="" class="navigation__list-link-top"> Возможности </a>
              </li>
              <li class="navigation__list-link-item">
                <a href="" class="navigation__list-link-top">
                  Как это работает?
                </a>
              </li>
            </ul>
          </div>
          <button  :class="['burger', { 'open': isMenuOpen }]" @click="toggleMenu">
            <span class="burger__line"></span>
          </button>
        </div>
        <div :class="['navigation__back', { 'open': isMenuOpen }]"></div>
      </div>
    </nav>
  </header>
</template>

<style scoped>
</style>