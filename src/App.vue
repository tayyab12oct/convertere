<template>
  <div class="">
    <Header />
    <HeaderSection />
    <div class="">
      <p class="">Jak działa Normobaria</p>
      <p class="">Warunki w komorze sprzyjają optymalnemu natlenieniu organizmu człowieka. Tlen jest łatwiej uwalniany
        z hemoglobiny oraz rozpuszczony w osoczu krwi. Wodór obecny w większym stężeniu działa antyoksydacyjnie,
        dezaktywuje wolne rodniki i korzystne wpływa
        w terapii wielu chorób.</p>
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
</script>
