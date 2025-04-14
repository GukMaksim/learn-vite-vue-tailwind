<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
  <header class="bg-base-100 shadow-md">
    <div class="container mx-auto px-4">
      <div class="navbar min-h-16">
        <!-- Логотип -->
        <div class="navbar-start">
          <div class="flex items-center">
            <img src="/vite.svg" alt="Logo" class="h-8 w-8 mr-2" />
            <span class="text-xl font-bold">Vue App</span>
          </div>
        </div>
        
        <!-- Мобільне меню -->
        <div class="navbar-end lg:hidden">
          <button class="btn btn-ghost" @click="toggleMenu">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>
        
        <!-- Десктопне меню -->
        <div class="navbar-center hidden lg:flex">
          <ul class="menu menu-horizontal px-1">
            <li><a href="#" class="active">Головна</a></li>
            <li><a href="#">Про нас</a></li>
            <li><a href="#">Послуги</a></li>
            <li><a href="#">Контакти</a></li>
          </ul>
        </div>
        
        <!-- Кнопки дій -->
        <div class="navbar-end hidden lg:flex">
          <button class="btn btn-primary mr-2">Увійти</button>
          <button class="btn btn-secondary">Реєстрація</button>
        </div>
      </div>
      
      <!-- Мобільне меню (випадаюче) -->
      <div v-if="isMenuOpen" class="lg:hidden py-2">
        <ul class="menu menu-vertical px-1">
          <li><a href="#" class="active">Головна</a></li>
          <li><a href="#">Про нас</a></li>
          <li><a href="#">Послуги</a></li>
          <li><a href="#">Контакти</a></li>
          <li class="mt-2">
            <button class="btn btn-primary w-full mb-2">Увійти</button>
            <button class="btn btn-secondary w-full">Реєстрація</button>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>