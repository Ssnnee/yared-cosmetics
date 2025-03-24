<script setup lang="ts">

defineProps<{ title: string, description: string, price: number, img: string, url: string }>()

</script>

<template>
  <div class="w-xs space-y-3 shadow-lg dark:shadow-none dark:border dark:border-border-d rounded-lg flex flex-col items-center p-8 ">
    <img :src="img" :alt="'picture of' + title" class="w-1/2" />
    <h3 class="text-xl font-bold w-full">{{ title }}</h3>
    <p class="w-full">{{ description }}</p>
    <p class="w-full text-xl  font-bold"> Price : {{ price }} FCFA</p>
    <button class="w-full flex items-center justify-center gap-3 cursor-pointer bg-violet text-white p-2 rounded-lg transform transition-all hover:scale-105">
      <a href="" class="">
        <img class="w-5" src="/icons/whatsapp-brands-light.svg" alt="Icons de whatsapp" />
      </a>
      <a :href="url">
        <p> Commander </p>
      </a>
    </button>
  </div>
</template>
