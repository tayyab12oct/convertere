<template>
    <div className="lg:px-9 px-5 lg:py-28 md:py-12 py-10 max-w-5xl w-full mx-auto">
        <ul class="flex md:space-x-12 space-x-6 lg:pb-16 md:pb-10 pb-6">
            <li class="cursor-pointer md:text-3xl sm:text-xl text-sm font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(1)" v-bind:class="{
                  'text-gray-300': openTab !== 1,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 1,
                }">
                Przebieg sesji
            </li>
            <li class="cursor-pointer md:text-3xl sm:text-xl text-sm font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(2)" v-bind:class="{
                  'text-gray-300': openTab !== 2,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 2,
                }">
                Jak to działa
            </li>
            <li class="cursor-pointer md:text-3xl sm:text-xl text-sm font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(3)" v-bind:class="{
                  'text-gray-300': openTab !== 3,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 3,
                }">
                Przygotowanie
            </li>
        </ul>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 1,
          block: openTab === 1,
        }">
            <p class="pr-14 md:leading-8 text-gray-600 md:text-xl text-sm">Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Molestias
                vel at quo esse sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias vel at quo esse
                sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus.</p>
            <div class="hidden md:flex">
                <div class="md:w-46 w-20"><img src="../assets/przy.png" alt="" class="w-46" /></div>
            </div>
        </div>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 2,
          block: openTab === 2,
        }">
            <p class="pr-14 md:leading-8 text-gray-600 md:text-xl text-sm">Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Molestias
                vel at quo esse sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias vel at quo esse
                sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa.</p>
            <div class="hidden md:flex">
                <div class="md:w-46 w-20"><img src="../assets/przy.png" alt="" class="w-46" /></div>
            </div>
        </div>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 3,
          block: openTab === 3,
        }">
            <p class="pr-14 md:leading-8 text-gray-600 md:text-xl text-sm">Do wizyty w komorze normobarycznej <b>nie trzeba się
                specjalnie przygotowywać</b> . Jeśli pacjent ma obawy bądź wątpliwości warto wspomóc się szeroko dostępną
                wiedzą na temat normo barii. Warto także <b>zadzwonić do nas</b> chętnie odpowiemy na nurtujące Państwa
                pytania, rozwiejemy wątpliwości.
                Jedyny <b>dyskomfort</b> związany z przygotowaniem do pobytu w komorze jest związany z adaptacją naszego
                organizmu do <b>zwiększającego się ciśnienia</b>. Tu należy wspomnieć co to za dyskonfort!!!!.</p>
            <div class="hidden md:flex">
                <div class="md:w-46 w-20"><img src="../assets/przy.png" alt="" class="w-46" /></div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';


const openTab = ref(1);
const toggleTabs = (id) => {
    openTab.value = id
}
</script>
