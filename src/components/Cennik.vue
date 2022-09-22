<template>
    <div class="md:px-12 px-5 md:pt-14 pt-16 max-w-6xl w-full mx-auto -mb-48 relative z-30">
        <h1 class="text-secondary-400 md:text-6xl text-5xl tracking-wide text-center font-bold">Cennik</h1>
        <p class="text-center text-gray-600 md:text-xl text-base max-w-4xl md:p-8 mx-auto md:pt-12 pt-6">Lorem ipsum dolor
            sit
            amet consectetur adipisicing elit.
        </p>
        <div class="grid md:grid-cols-2 lg:gap-8 gap-6 pt-14 pb-12">
            <TableCard />
            <TableCard />
        </div>
    </div>
    <div class="relative border">
        <img src="../assets/mid-bg.png" alt="midBG" class="absolute inset-x-0 top-0 w-full" />
        <div class="md:px-12 px-5 pt-42 max-w-6xl w-full mx-auto relative z-30">
            <p class="text-primary-100 text-xl tracking-wide text-center pt-10 uppercase">PROMOCJA MIESIĄCA</p>
            <p class="text-center text-white md:text-4xl text-2xl py-3 font-bold">Przedsprzedaż -50% za 1 wejście</p>
            <p class="text-primary-100 text-2xl text-center pt-2 max-w-3xl mx-auto">Lorem ipsum dolor sit amet, consectetur adipiscing
                elit. Donec porttitor
                ligula et ex tincidunt euismod. <b>Praesent faucibus</b> diam eget justo pharetra,
                ac laoreet ligula rutrum.</p>
            <div class="grid md:grid-cols-2 lg:gap-8 gap-6 pt-12 pb-12">
                <TableCard />
                <TableCard />
            </div>
        </div>
    </div>
</template>

<script setup>
import TableCard from './TableCard.vue';
</script>