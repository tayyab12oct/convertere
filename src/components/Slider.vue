<template>
    <Carousel :wrapAround="true" :breakpoints="breakpoints">
        <template #addons>
            <Pagination />
        </template>
        <Slide v-for="slide in 5" :key="slide">
            <div class="carousel__item rounded-2xl shadow-lg w-full overflow-hidden">
                <img src="../assets/slider/mid.png" class="w-full h-full" alt="">
            </div>
        </Slide>
    </Carousel>
</template>
  
<script setup>
import { Carousel, Pagination, Slide } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';
const breakpoints = {
    1280: {
        itemsToShow: 2,
    },
    1024: {
        itemsToShow: 1.7,
    },
    768: {
        itemsToShow: 1.15,
    },
    200: {
        itemsToShow: 1.01,
    },
}
</script>
  
<style scope>
.carousel__item {
    @apply xl:h-auto lg:h-auto lg:border border-red-500 md:h-[400px];
}

.carousel__slide {
    @apply px-8 xl:h-[65vh] lg:h-auto sm:h-[60vh] md:h-[55vh] md:mt-14 mt-5;
}

.carousel__pagination {
    @apply absolute top-0 mb-10 inset-x-0 w-full
}

.carousel__pagination-item .carousel__pagination-button {
    @apply bg-gray-800 md:w-16 w-12 sm:mx-3 mx-1.5
}

.carousel__pagination-item .carousel__pagination-button--active {
    @apply bg-secondary-100
}

.carousel__slide>.carousel__item {
    transform: scale(1);
    transition: 0.5s;
}

.carousel__slide--next>.carousel__item {
    transform: scale(0.9) translate(-10px);
}

.carousel__slide--prev>.carousel__item {
    transform: scale(0.9) translate(10px);
}

.carousel__slide--active>.carousel__item {
    transform: scale(1.1);
    @apply my-10;
}
</style>