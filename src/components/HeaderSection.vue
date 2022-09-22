<template>
    <div class="relative pb-20 overflow-x-hidden">
        <img src="../assets/top-bg.png" alt="" class="absolute top-0 inset-x-0 w-full h-full" />
        <div className="max-w-6xl w-full mx-auto flex md:flex-row flex-col justify-between relative">
            <div class="lg:max-w-xl max-w-lg lg:px-12 px-5 lg:py-20 md:py-12 py-10 relative z-30">
                <p
                    className="text-primary-100 lg:text-[3.85rem] lg:leading-[4.5rem] text-5xl tracking-wider font-bold lg:pr-5 md:pr-10">
                    Normobaria.
                    Co to jest?
                </p>
                <p class="text-gray-600 md:text-xl text-lg lg:py-12 py-10 md:pr-14">Lorem ipsum dolor sit amet,
                    consectetur
                    adipiscing elit. Curabitur sit amet egestas libero. Nam varius faucibus ipsum. Integer et nisi
                    porta, ornare risus nec, eleifend.
                </p>
                <button type="submit"
                    className="xl:mt-16 lg:mt-3 mb-8 lg:mb-0 flex items-center justify-center rounded-full whitespace-nowrap border border-transparent bg-blue-100 px-6 md:py-4 py-3 tracking-wider lg:text-lg md:text-base text-sm uppercase font-bold text-white focus:outline-none">
                    Umów wizytę
                    <img src="../assets/arrow-right-white.png" alt="arrow-right" class="w-5 ml-3" />
                </button>
            </div>
            <div className="xl:-mr-40 md:-ml-30 lg:-mb-10 md:pt-11 pt-8 pr-5 md:pr-0 relative z-30 sm:pl-20 md:pl-0 hidden md:block">
                <img src="../assets/header-img.png" class="" alt="HeaderImg">
            </div>
        </div>
    </div>
</template>
