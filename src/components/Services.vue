<template>
    <div class="relative -mt-38 pt-40 z-20">
        <img src="../assets/newsletter.jpeg" class="absolute inset-0 w-full h-full" alt="Newsletter">
        <div className="relative lg:px-9 px-5 lg:py-22 md:py-12 py-10 max-w-6xl w-full mx-auto">
            <p className="text-white lg:text-6xl text-3xl tracking-wide font-bold text-center">
                Dla kogo Normobaria?
            </p>
            <div class="grid md:grid-cols-3 grid-cols-1 gap-5 md:pt-22 pt-10 -mb-46">
                <div class="bg-white rounded-2xl lg:p-9 p-6 shadow-lg flex flex-col items-start" v-for="v in services"
                    :key="v">
                    <div class="lg:h-22 h-12">
                        <img :src="v.src" :class="v.imgClass" alt="icon" />
                    </div>
                    <p
                        class="font-bold text-primary-100 lg:px-5.5 px-3 lg:-mx-5.5 -mx-3 pt-12 mb-4 leading-2 text-2xl border-b-[20px] border-secondary-500">
                        {{v.title}}</p>
                    <p class="text-sm text-gray-600">{{v.desc}}</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import card1 from "../assets/card-1.png"
import card2 from "../assets/card-2.png"
import card3 from "../assets/card-3.png"
const services = [
    {
        src: card1,
        imgClass: "lg:w-20 w-14",
        title: "Dla",
        desc: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae."
    },
    {
        src: card2,
        imgClass: "lg:w-22 w-14",
        title: "Dla",
        desc: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae."
    },
    {
        src: card3,
        imgClass: "lg:w-16 w-12",
        title: "Dla",
        desc: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus autem mollitia possimus animi voluptatem odit ducimus pariatur rem ullam perspiciatis expedita quae nulla obcaecati, voluptas commodi explicabo nobis. Quibusdam, molestiae."
    },
]
</script>
