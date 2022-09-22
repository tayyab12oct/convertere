<template>
    <div class="lg:px-12 px-5 md:pt-14 pt-16 max-w-6xl w-full mx-auto 2xl:-mb-48 md:-mb-20 relative z-30">
        <h1 class="text-secondary-400 md:text-6xl text-5xl tracking-wide text-center font-bold">Cennik</h1>
        <p class="text-center text-gray-600 md:text-xl text-base max-w-4xl md:p-8 mx-auto md:pt-12 pt-6">Lorem ipsum
            dolor
            sit
            amet consectetur adipisicing elit.
        </p>
        <div class="grid md:grid-cols-2 lg:gap-8 gap-6 pt-14 pb-12">
            <TableCard />
            <TableCard />
        </div>
    </div>
    <div class="relative border">
        <img src="../assets/mid-bg.png" alt="midBG" class="absolute inset-x-0 top-0 w-full hidden md:block" />
        <div class="lg:px-12 px-5 xl:pt-16 2xl:pt-42 md:pt-4 max-w-6xl w-full mx-auto relative z-30">
            <p class="text-primary-100 text-xl tracking-wide text-center lg:pt-10 md:pt-16 uppercase">PROMOCJA MIESIĄCA</p>
            <p class="text-center md:text-white text-secondary-400 lg:text-4xl md:text-3xl text-2xl lg:py-3 py-2 font-bold">Przedsprzedaż -50% za 1 wejście</p>
            <p class="text-primary-100 lg:text-2xl text-base text-center lg:pt-2 max-w-3xl mx-auto">Lorem ipsum dolor sit amet,
                consectetur adipiscing
                elit. Donec porttitor
                ligula et ex tincidunt euismod. <b>Praesent faucibus</b> diam eget justo pharetra,
                ac laoreet ligula rutrum.</p>
            <div class="grid md:grid-cols-2 lg:gap-8 gap-6 pt-12 lg:pb-8 pb-6">
                <TableCard />
                <TableCard />
            </div>
            <div class="grid md:grid-cols-5 items-start lg:gap-8 gap-6">
                <div class="bg-white shadow-md md:py-8 md:px-9 p-5 rounded-2xl md:col-span-3">
                    <h1 class="text-primary-100 md:text-2xl text-lg uppercase tracking-wide pb-6"><b>Strefa Standard
                            /</b> sesja nocna</h1>
                    <table class="min-w-full">
                        <thead>
                            <tr>
                                <th scope="col"
                                    class="md:py-3.5 py-2 pl-0 pr-3 text-left text-sm md:text-base font-semibold text-secondary-400">
                                    Lorem ipsum
                                </th>
                                <th scope="col"
                                    class="md:py-3.5 py-2 pl-3 pr-0 text-right text-sm md:text-base font-semibold text-secondary-400">
                                    Rabat
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr v-for="project in projects" :key="project.id" class="border-b border-gray-400">
                                <td class="py-4 pr-3 text-sm md:text-base pl-0">
                                    <div class="font-medium text-gray-600"><span class="pr-2">{{project.id}}</span> {{
                                    project.name }}</div>
                                </td>
                                <td
                                    class="py-4 pl-3 pr-4 text-right text-sm md:text-base text-gray-600 sm:pr-6 md:pr-0">
                                    {{
                                    project.rabat }}</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                <div class="bg-white shadow-md md:py-8 md:px-9 p-5 pb-0 md:pb-0 rounded-2xl md:col-span-2">
                    <h1 class="text-primary-100 md:text-2xl text-lg uppercase tracking-wide pb-6 font-bold">Rejestracja
                    </h1>
                    <p class="text-gray-600 md:text-lg text-sm py-0.5">Tel: <span class="font-semibold">+48 123 123 123</span></p>
                    <p class="text-gray-600 md:text-lg text-sm py-0.5">Email: <span
                            class="font-semibold">rejestracja@convertere.pl</span></p>
                    <p class="text-gray-600 md:text-lg text-sm pb-0.5 pt-8">lub zarejestruj się przez</p>
                    <p class="text-gray-600 md:text-lg text-sm pt-0.5 pb-10">aplikacje <span class="font-semibold">nazwa
                            apki</span></p>
                    <div class="flex justify-center -mb-7">
                        <button type="submit"
                            className="flex items-center justify-center rounded-full whitespace-nowrap bg-secondary-400 px-6 md:px-8 md:py-4.5 py-3 tracking-wider lg:text-lg md:text-base text-sm uppercase font-bold text-primary-100 focus:outline-none">
                            Umów wizytę
                            <img src="../assets/arrow-right-primary.png" alt="arrow-right" class="w-4 ml-3" />
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import TableCard from './TableCard.vue';
const projects = [
    { id: 1, name: 'sesja w normobarii ', rabat: '499 zt' },
    { id: 2, name: 'sesj w normobarii ', rabat: '499 zt' },
    { id: 3, name: 'sesj w normobarii ', rabat: '499 zt' },
    { id: 4, name: 'sesj w normobarii ', rabat: '499 zt' },
]
</script>