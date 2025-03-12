<script setup lang="ts">

defineProps<{ caterory?: string, title: string, description: string, price: number, img: string }>()

</script>

<template>
  <div class="w-xs space-y-3 shadow-lg dark:shadow-none dark:bg-foreground  rounded-lg flex flex-col items-center p-8 ">
    <h2 class="text-2xl w-full font-bold">{{ caterory }}</h2>
    <img :src="img" :alt="'picture of' + title" class="w-1/2" />
    <h3 class="text-xl font-bold w-full">{{ title }}</h3>
    <p class="w-full">{{ description }}</p>
    <p class="w-full text-xl  font-bold"> Price : {{ price }} FCFA</p>
    <button class="w-full cursor-pointer bg-violet text-white p-2 rounded-lg transform transition-all hover:scale-105">
      Command
    </button>
  </div>
</template>
