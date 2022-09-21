<template>
    <div className="md:px-9 px-5 lg:py-28 md:py-12 py-10 max-w-5xl w-full mx-auto">
        <ul class="flex space-x-12 pb-16">
            <li class="cursor-pointer text-3xl font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(1)" v-bind:class="{
                  'text-gray-300': openTab !== 1,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 1,
                }">
                Tab 1
            </li>
            <li class="cursor-pointer text-3xl font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(2)" v-bind:class="{
                  'text-gray-300': openTab !== 2,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 2,
                }">
                Tab 2
            </li>
            <li class="cursor-pointer text-3xl font-bold pb-1 transition-all border-b-4 border-transparent"
                v-on:click="toggleTabs(3)" v-bind:class="{
                  'text-gray-300': openTab !== 3,
                  'text-primary-100 border-secondary-400 transition-all': openTab === 3,
                }">
                Tab 3
            </li>
        </ul>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 1,
          block: openTab === 1,
        }">
            <p class="pr-7 text-gray-600 text-xl">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias
                vel at quo esse sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias vel at quo esse
                sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus.</p>
            <div class="hidden md:flex">
                <div class="w-46"><img src="../assets/przy.png" alt="" class="w-46" /></div>
            </div>
        </div>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 2,
          block: openTab === 2,
        }">
            <p class="pr-7 text-gray-600 text-xl">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias
                vel at quo esse sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias vel at quo esse
                sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa.</p>
            <div class="hidden md:flex">
                <div class="w-46"><img src="../assets/przy.png" alt="" class="w-46" /></div>
            </div>
        </div>
        <div class="flex items-start" v-bind:class="{
          hidden: openTab !== 3,
          block: openTab === 3,
        }">
            <p class="pr-7 text-gray-600 text-xl">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias
                vel at quo esse sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum quae
                culpa repellendus. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestias vel at quo esse
                sit dolore
                voluptatibus quasi error accusantium, deleniti delectus maiores eveniet quas, molestiae sed harum repellendus.</p>
            <div class="hidden md:flex">
                <div class="w-46"><img src="../assets/przy.png" alt="" class="w-46" /></div>
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
