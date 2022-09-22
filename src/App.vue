<template>
  <div class="overflow-x-hidden">
    <Header />
    <HeaderSection />
    <div class="text-center md:pb-32 pb-8 px-5 lg:px-0 relative">
      <img src="./assets/normobaria.png" alt="normobaria" class="absolute left-0 w-56 top-0 hidden xl:block" />
      <img src="./assets/right-bars.png" alt="right-bars" class="absolute right-0 w-32 top-1/2 hidden xl:block" />
      <div class="relative">
        <p class="text-primary-100 text-xl tracking-wide uppercase">Jak działa Normobaria</p>
        <hr class="bg-secondary-200 w-32 p-0.5 mx-auto my-7 border-1 border-transparent" />
        <p
          class="text-primary-100 font-semibold lg:text-4xl md:text-3xl text-xl max-w-5xl mx-auto w-full lg:leading-[2.85rem] md:leading-10 pt-4">
          Warunki w
          komorze sprzyjają optymalnemu
          natlenieniu organizmu człowieka. Tlen jest łatwiej uwalniany
          <br />z hemoglobiny oraz rozpuszczony w osoczu krwi. <br /> Wodór obecny w większym stężeniu działa
          antyoksydacyjnie, dezaktywuje wolne rodniki i korzystne wpływa <br />w terapii wielu chorób.
        </p>
      </div>
    </div>
    <CZY />
    <Tabs />
    <div class="relative z-30">
      <Slider />
    </div>
    <Services />
    <div class="bg-gray-250 md:pt-36 py-28 relative">
      <Cennik />
      <img src="./assets/tio.png" alt="tio" class="absolute inset-x-0 min-w-[110%] bottom-72 -mx-22 hidden xl:block" />
    </div>
    <Newsletter />
    <Contact />
    <Footer />
  </div>
</template>
<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Contact from "./components/Contact.vue";
import Newsletter from "./components/Newsletter.vue";
import HeaderSection from "./components/HeaderSection.vue";
import CZY from "./components/CZY.vue";
import Tabs from "./components/Tabs.vue";
import Slider from "./components/Slider.vue";
import Services from "./components/Services.vue";
import Cennik from "./components/Cennik.vue";
</script>
