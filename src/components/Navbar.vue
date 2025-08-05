<template>
  <header class="fixed top-0 left-0 w-full z-50 bg-white/80 backdrop-blur shadow-sm">
    <nav class="max-w-7xl mx-auto px-4 py-4 flex items-center justify-between">
      <!-- Logo -->
      <h1 class="text-2xl font-bold text-orange-500">Huellas Vivas</h1>

      <!-- Botón hamburguesa (solo en móvil) -->
      <button
        class="md:hidden text-gray-700 focus:outline-none"
        @click="menuAbierto = !menuAbierto"
      >
        <svg
          v-if="!menuAbierto"
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
        <svg
          v-else
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>
      </button>

      <!-- Menú horizontal en escritorio -->
      <ul class="hidden md:flex space-x-6 text-gray-700 font-medium items-center">
        <li><a href="#nosotros" class="hover:text-orange-500 transition">Sobre Nosotros</a></li>
        <li><a href="#perritos" class="hover:text-orange-500 transition">Perritos</a></li>
        <li><a href="#adopcion" class="hover:text-orange-500 transition">Adopción</a></li>
        <li><a href="#contacto" class="hover:text-orange-500 transition">Contacto</a></li>
        <li>
          <a
            href="#adoptar"
            class="bg-orange-500 text-white font-semibold px-5 py-2 rounded hover:bg-orange-600 transition"
          >
            Adoptar
          </a>
        </li>
      </ul>
    </nav>

    <!-- Menú desplegable en móvil -->
    <div
      v-if="menuAbierto"
      class="md:hidden px-4 py-4 bg-white/80 backdrop-blur border-t border-gray-200"
    >
      <ul class="flex flex-col gap-4 text-gray-700 font-medium">
        <li><a href="#nosotros" class="hover:text-orange-500 transition">Sobre Nosotros</a></li>
        <li><a href="#perritos" class="hover:text-orange-500 transition">Perritos</a></li>
        <li><a href="#adopcion" class="hover:text-orange-500 transition">Adopción</a></li>
        <li><a href="#contacto" class="hover:text-orange-500 transition">Contacto</a></li>
        <li>
          <a
            href="#adoptar"
            class="block text-center bg-orange-500 text-white font-semibold px-5 py-2 rounded hover:bg-orange-600 transition"
          >
            Adoptar
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const menuAbierto = ref(false)
</script>
