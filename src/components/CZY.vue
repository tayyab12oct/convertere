<template>
    <div class="relative md:pt-20 lg:pb-20 bg-gray-200 md:bg-transparent overflow-x-hidden">
        <img src="../assets/mid-round-bg.png" class="absolute border top-0 inset-0 w-full h-full hidden md:block" alt="Gradient" />
        <div className="max-w-6xl w-full mx-auto flex lg:flex-row flex-col items-start justify-between relative">
            <div class="max-w-3xl lg:pr-10 lg:pl-20 px-5 lg:py-20 md:pb-24 py-20 relative z-30">
                <p class="md:text-xl text-lg pb-8 uppercase text-gray-600">Czy wiesz że</p>
                <p
                    className="text-primary-100 lg:text-4xl md:text-3xl text-xl tracking-wide font-semibold lg:leading-10 lg:pr-10 xl:pr-0">
                    W komorze normobarycznej panuje podwyższone ciśnienie 1500 hpa, dla porównania ciśnienie w
                    atmosferze ziemskiej wynosi około 1000 hpa.
                </p>
                <p
                    className="text-primary-100 lg:text-4xl md:text-3xl text-xl tracking-wide font-semibold md:pt-18 pt-12">
                    Normobaria w liczbach:
                </p>
                <div class="grid md:grid-cols-2 gap-18 pt-14">
                    <div class="" v-for="v in data" :key="v">
                        <p class="md:text-xl text-lg pb-2 text-primary-100 tracking-wide">{{v.title}}</p>
                        <p class="md:text-5xl text-4xl font-bold text-secondary-300 pb-5">{{v.span}}</p>
                        <div class="bg-primary-100 w-full h-3">
                            <div class="bg-secondary-300 h-full" :style="{width: v.width}"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div className="xl:-mr-44 -mt-14 relative z-30 hidden lg:block">
                <img src="../assets/side.png" class="" alt="HeaderImg">
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
