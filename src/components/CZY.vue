<template>
    <div class="relative bg-gray-200 pb-20 rounded-tr-[50%]">
        <div className="max-w-6xl w-full mx-auto flex lg:flex-row flex-col items-start justify-between">
            <div class="max-w-3xl md:px-20 px-5 lg:py-20 md:py-12 py-10 relative z-30">
                <p class="text-xl pb-8 uppercase text-gray-600">Czy wiesz że</p>
                <p
                    className="text-primary-100 lg:text-4xl md:text-3xl text-2xl tracking-wide font-semibold lg:leading-10">
                    W komorze normobarycznej panuje podwyższone ciśnienie 1500 hpa, dla porównania ciśnienie w
                    atmosferze ziemskiej wynosi około 1000 hpa.
                </p>
                <p className="text-primary-100 lg:text-4xl md:text-3xl text-2xl tracking-wide font-semibold pt-18">
                    Normobaria w liczbach:
                </p>
                <div class="grid grid-cols-2 gap-18 pt-14">
                    <div class="" v-for="v in data" :key="v">
                        <p class="text-xl pb-2 text-gray-600">{{v.title}}</p>
                        <p class="text-6xl font-bold text-secondary-300 pb-5">{{v.span}}</p>
                        <div class="bg-primary-100 w-full h-3">
                            <div class="bg-secondary-300 h-full" :style="{width: v.width}"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div className="-mr-56 -ml-20 -mt-20 relative z-30">
                <img src="../assets/czy.jpeg" class="" alt="HeaderImg">
            </div>
        </div>
    </div>
</template>
<script setup>
const data = [
    {
        title: "Stężenie tlenu",
        width: "40%",
        span: "32-40%"
    },
    {
        title: "Stężenie wodoru",
        width: "3%",
        span: "0,5%"
    },
    {
        title: "Stężenie wutlenku węgla",
        width: "4%",
        span: "07-1,3%"
    },
    {
        title: "Czas trwania sesji",
        width: "95%",
        span: "120 min"
    },
]
</script>
