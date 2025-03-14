<script setup lang="ts">
</script>

<template>
  <div className="flex items-center justify-between px-14">
    <div class="flex items-center w-full space-x-4">
      <div class="border-b dark:border-border-d w-1/2"></div>
      <a href="" class="">
        <img class="w-8" src="/logo.png" alt="" />
      </a>
      <div class="border-b dark:border-border-d w-1/2"></div>
      </hr>
    </div>
  </div>
  <footer className="flex items-center justify-between px-14 m-2">
    <p>© {{ new Date().getFullYear() }} Yared Cosmetecs</p>
    <div class="flex items-center space-x-4 dark:hidden">
      <a href="" class="">
        <img class="w-5" src="/icons/envelope-regular.svg" alt="Icons de mail" />
      </a>
      <a href="https://www.instagram.com/yaredcosmetics" class="">
        <img class="w-5" src="/icons/instagram-brands.svg" alt="Icons de instagram" />
      </a>
      <a href="https://wa.me/242053782440" class="">
        <img class="w-5" src="/icons/whatsapp-brands.svg" alt="Icons de whatsapp" />
      </a>
      <a href="https://www.facebook.com/share/195bMy9xWJ/?mibextid=wwXIfr" class="">
        <img class="w-5" src="/icons/facebook-brands.svg" alt="Icons de facebook" />
      </a>
    </div>

      <!-- For the dark mode -->
    <div class="dark:flex items-center space-x-4 hidden">
      <a href="" class="">
        <img class="w-5" src="/icons/envelope-regular-light.svg" alt="Icons de mail" />
      </a>
      <a href="https://www.instagram.com/yaredcosmetics" class="">
        <img class="w-5" src="/icons/instagram-brands-light.svg" alt="Icons de instagram" />
      </a>
      <a href="https://wa.me/242053782440" class="">
        <img class="w-5" src="/icons/whatsapp-brands-light.svg" alt="Icons de whatsapp" />
      </a>
      <a href="https://www.facebook.com/share/195bMy9xWJ/?mibextid=wwXIfr" class="">
        <img class="w-5" src="/icons/facebook-brands-light.svg" alt="Icons de facebook" />
      </a>
    </div>
  </footer>
</template>

