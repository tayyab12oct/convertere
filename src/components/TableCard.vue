<template>
    <div class="bg-white shadow-md md:py-8 md:px-9 p-5 rounded-2xl">
        <h1 class="text-primary-100 md:text-2xl text-lg uppercase tracking-wide pb-6"><b>Strefa Standard /</b> sesja nocna</h1>
        <table class="min-w-full">
            <thead>
                <tr>
                    <th scope="col"
                        class="md:py-3.5 py-2 pl-0 pr-3 text-left text-sm md:text-base font-semibold text-secondary-400">Ilość
                        sesji
                    </th>
                    <th scope="col"
                        class="hidden md:py-3.5 py-2 px-3 text-right text-sm md:text-base font-semibold text-secondary-400 sm:table-cell">
                        Czas
                    </th>
                    <th scope="col"
                        class="md:py-3.5 py-2 pl-3 pr-0 text-right text-sm md:text-base font-semibold text-secondary-400">Cena
                    </th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="project in projects" :key="project.id" class="border-b border-gray-400">
                    <td class="py-4 pl-4 pr-3 text-sm md:text-base sm:pl-6 md:pl-0">
                        <div class="font-medium text-gray-600"><span class="pr-2">{{project.id}}</span> {{
                        project.name }}</div>
                    </td>
                    <td class="hidden py-4 px-3 text-right text-sm md:text-base text-gray-600 sm:table-cell">{{
                    project.czas }}</td>
                    <td class="py-4 pl-3 pr-4 text-right text-sm md:text-base text-gray-600 sm:pr-6 md:pr-0">{{
                    project.cena }}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script setup>
const projects = [
    { id: 1, name: 'sesja w normobarii ', czas: '12 h', cena: '499 zt' },
    { id: 2, name: 'sesj w normobarii ', czas: '12 h', cena: '499 zt' },
    { id: 3, name: 'sesj w normobarii ', czas: '12 h', cena: '499 zt' },
    { id: 4, name: 'sesj w normobarii ', czas: '12 h', cena: '499 zt' },
]
</script>