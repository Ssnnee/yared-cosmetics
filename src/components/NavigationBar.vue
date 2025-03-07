<script setup lang="ts">
import { ref } from 'vue';

 const navigation = ref([
    { name: 'Home', href: '/home' },
    { name: 'About', href: '/about' },
    { name: 'Contact', href: '/contact' },
  ])
</script>

<template>
  <header class="py-4 border-b">
    <nav class="flex container items-center">
      <a href="" class="flex gap-1 items-center">
        <img class="w-14" src="/logo.png" alt="" />
        <span class="text-3xl font-bold">Nuxtcipes</span>
      </a>
      <ul class="flex gap-6 ml-auto text-xl font-bold capitalize">
        <li>
          <a href="">Home</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

