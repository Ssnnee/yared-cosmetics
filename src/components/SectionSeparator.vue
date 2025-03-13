<script setup lang="ts">

defineProps<{ sectionTitle: string }>()

</script>

<template>
  <div class="flex flex-col items-center justify-center">
    <div class="border-b dark:border-border-d w-1/2"></div>
    <h2 class="text-4xl my-10">{{ sectionTitle }}</h2>
  </div>
</template>
