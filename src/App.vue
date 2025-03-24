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
            Ingrédients purs, résultats puissants. Nourrissez vos cheveux de manière naturelle.
          </p>
          <a href="#A propos">
            <button class="w-xs bg-violet text-white p-2 rounded-lg cursor-pointer transform transition-all hover:scale-105">
              En savoir plus
            </button>
          </a>
        </div>
        <div class="order-first lg:order-last">
          <img src="/actor.png" alt="" />
        </div>
      </div>
    </section>
    <section id="Produit">
      <SectionSeparator sectionTitle="Hair Products" />
      <div class="flex flex-wrap justify-center gap-4">
        <ProductCard
          title="Chebe Oil"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 2500
          img="/chebe-oil.png"
          url="https://wa.me/p/28794389326842425/242053782440"
        />
        <ProductCard
          title="Hair Tonic Spray"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 2000
          img="clove-hair-tonic.png"
          url="https://wa.me/p/9358370687544442/242053782440"
        />
        <ProductCard
          title="Natural Shampoo"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 4000
          img="shampoon.png"
          url="https://wa.me/p/9594573337261297/242053782440"
        />
        <ProductCard
          title="Hair Traitment"
          description="Our shampoo is made with natural ingredients that will leave your hair feeling clean and refreshed."
          :price= 2500
          img="hair-traitment.png"
          url="https://wa.me/p/9666309590097738/242053782440"
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
