<script setup lang="ts">
  const navItems = ["Accueil","Produit", "A propos" , "Contact",];
</script>

<template>
  <header class="py-4 px-14">
    <nav class="flex flex-center justify-between ">
      <a href="" class="">
        <img class="w-14" src="/logo.png" alt="" />
      </a>
      <ul class="flex flex-center space-x-4 ">
        <li v-for="item in navItems" :key="item">
          <a :href="'#' + item">{{ item }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

