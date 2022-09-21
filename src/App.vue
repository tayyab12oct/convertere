<template>
  <div class="">
    <Header />
    <HeaderSection />
    <div class="text-center pb-20 relative">
      <img src="./assets/normobaria.png" alt="normobaria" class="absolute left-0 w-56 top-0" />
      <p class="text-primary-100 text-xl tracking-wide uppercase">Jak działa Normobaria</p>
      <hr class="bg-secondary-200 w-32 p-0.5 mx-auto my-7 border-1 border-transparent" />
      <p class="text-primary-100 font-semibold text-4xl max-w-5xl mx-auto w-full leading-[2.85rem] pt-4">Warunki w
        komorze sprzyjają optymalnemu
        natlenieniu organizmu człowieka. Tlen jest łatwiej uwalniany
        z hemoglobiny oraz rozpuszczony w osoczu krwi. <br> Wodór obecny w większym stężeniu działa antyoksydacyjnie,
        dezaktywuje wolne rodniki i korzystne wpływa
        w terapii wielu chorób.</p>
    </div>
    <CZY />
    <Tabs />
    <div class="relative z-30"><Slider /></div>
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
</script>
