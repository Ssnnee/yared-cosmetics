<script setup lang="ts">
import { ref } from 'vue';

const navItems = ["Accueil", "Produit", "A propos", "Contact"];
const isMenuOpen = ref(false);
</script>

<template>
  <header class="py-4 px-14">
    <nav class="flex justify-between items-center">
      <a href="">
        <img class="w-20" src="/logo.png" alt="Logo" />
      </a>

      <!-- Desktop Menu -->
      <ul class="hidden md:flex space-x-6">
        <li v-for="item in navItems" :key="item">
          <a :href="'#' + item" class="hover:text-violet">{{ item }}</a>
        </li>
      </ul>

      <button @click="isMenuOpen = !isMenuOpen" class="md:hidden cursor-pointer">
        <img v-if="!isMenuOpen" class="w-8 flex dark:hidden" src="/icons/menu.svg" alt="Menu" />
        <img v-if="!isMenuOpen" class="w-8 hidden dark:flex" src="/icons/menu-light.svg" alt="Menu" />
        <img v-if="isMenuOpen" class="w-8 flex dark:hidden" src="/icons/close.svg" alt="Menu" />
        <img v-if="isMenuOpen" class="w-8 hidden dark:flex" src="/icons/close-light.svg" alt="Menu" />
      </button>
    </nav>

    <!-- Mobile Menu -->
    <div v-if="isMenuOpen" class="md:hidden mt-4 transition-all delay-1000 absolute">
      <ul class="flex flex-col space-y-4 p-4 shadow-lg">
        <li v-for="item in navItems" :key="item">
          <button @click="isMenuOpen = !isMenuOpen" class="cursor-pointer">
            <a :href="'#' + item" class="hover:text-violet">{{ item }}</a>
          </button>
        </li>
      </ul>
    </div>
  </header>
</template>

