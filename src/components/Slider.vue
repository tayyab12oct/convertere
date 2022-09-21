<template>
    <Carousel :itemsToShow="2" :wrapAround="true">
        <template #addons>
            <Pagination />
        </template>
        <Slide v-for="slide in 5" :key="slide">
            <div class="carousel__item rounded-2xl shadow-lg w-full overflow-hidden">
                <img src="../assets/czy.jpeg" class="w-full h-full" alt="">
            </div>
        </Slide>

    </Carousel>
</template>
  
<script setup>
import { Carousel, Pagination, Slide } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';
</script>
  
<style scope>
.carousel__item {
    height: 535px;
}

.carousel__slide {
    @apply px-8 h-[65vh] mt-14;
}

.carousel__pagination {
    @apply absolute top-0 mb-10 inset-x-0 w-full
}

.carousel__pagination-item .carousel__pagination-button {
    @apply bg-gray-700 w-18 mx-4
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