<script setup lang="ts">
import NavigationBar from './components/NavigationBar.vue';
import Footer from './components/Footer.vue';
import ProductCard from './components/ProductCard.vue';
import SectionSeparator from './components/SectionSeparator.vue';

</script>

<template>
  <NavigationBar />
  <main class="flex flex-col justify-center items-center">
    <section id="Accueil">
      <div class="flex justify-center items-center flex-col lg:flex-row gap-12 m-10">
        <div class="lg:w-2xl flex-1 lg:flex-initial flex items-center lg:items-start flex-col gap-5 text-center lg:text-left">
          <h1 class="text-4xl lg:text-6xl font-kaushan">
            Natural product for the most efficient result
          </h1>
          <p class="lg:w-sm text-xl">
            Pure ingredients, powerful results—nourish your hair the natural way.
          </p>
          <a href="#A propos">
            <button class="w-xs bg-violet text-white p-2 rounded-lg cursor-pointer transform transition-all hover:scale-105">
              More about us
            </button>
          </a>
        </div>
        <div class="order-first lg:order-last">
          <img src="/actor.png" alt="" />
        </div>
      </div>
    </section>
    <section id="Produit">
      <SectionSeparator sectionTitle="Products" />
      <div class="flex flex-wrap justify-center gap-4">
        <ProductCard
          caterory="Hair Care"
          title="Shampoo"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 100
          img="/chebe-oil.png"
        />
        <ProductCard
          caterory="Hair Care"
          title="Shampoo"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 100
          img="clove-hair-tonic.png"
        />
        <ProductCard
          caterory="Hair Care"
          title="Shampoo"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 100
          img="shampoon.png"
        />
        <ProductCard
          caterory="Hair Care"
          title="Shampoo"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 100
          img="hair-traitment.png"
        />
      </div>
    </section>
    <section id="A propos" class="my-10">
      <SectionSeparator sectionTitle="About" />
      <div class="flex flex-col items-center">
        <p class="w-full text-center text-2xl">
          “Natural does not kill”
        </p>
      </div>
      <div class="flex flex-col items-center gap-5">
        <img src="/logo.png" alt="" class="w-72" />
        <div class="flex items-center justify-between text-left w-1/2 gap-16">
          <p class="">
            Yared Cosmetics is a family-owned business that has been making natural hair care products for over 20 years.
          </p>
          <p class="">
            Yared Cosmetics is a family-owned business that has been making natural hair care products for over 20 years.
          </p>
        </div>
      </div>
    </section>
  </main>
  <Footer />
</template>
