<script setup>
import { ref } from 'vue'
import TheHeader from './components/TheHeader.vue'

const count = ref(0)
</script>

<template>
  <div class="min-h-screen bg-base-100">
    <TheHeader />
    
    <div class="container mx-auto px-4 py-8">
      <h1 class="text-4xl font-bold text-center mb-8">
        Vite + Vue + Tailwind + DaisyUI
      </h1>
      
      <div class="card w-96 bg-base-200 shadow-xl mx-auto">
        <div class="card-body">
          <h2 class="card-title">Лічильник</h2>
          <p class="text-center text-2xl font-bold">{{ count }}</p>
          <div class="card-actions justify-center mt-4">
            <button class="btn btn-primary" @click="count++">
              Збільшити
            </button>
            <button class="btn btn-secondary" @click="count--">
              Зменшити
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
