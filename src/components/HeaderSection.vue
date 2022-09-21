<template>
    <div class="relative bg-secondary-400 pb-20">
        <div className="max-w-6xl w-full mx-auto flex lg:flex-row flex-col items-center justify-between">
            <div class="max-w-xl md:px-12 px-5 lg:py-20 md:py-12 py-10 relative z-30">
                <p
                    className="text-primary-100 lg:text-[3.85rem] lg:leading-[4.5rem] md:text-3xl text-2xl tracking-wider font-bold pr-5">
                    Normobaria.
                    Co to jest?
                </p>
                <p class="text-gray-600 md:text-xl text-base py-12 md:pr-14">Lorem ipsum dolor sit amet, consectetur
                    adipiscing elit. Curabitur sit amet egestas libero. Nam varius faucibus ipsum. Integer et nisi
                    porta, ornare risus nec, eleifend.
                </p>
                <button type="submit"
                    className="mt-16 flex items-center justify-center rounded-full whitespace-nowrap border border-transparent bg-blue-100 px-6 py-4 tracking-wider lg:text-lg md:text-base text-sm uppercase font-bold text-white focus:outline-none">
                    Umów wizytę
                    <img src="../assets/arrow-right-white.png" alt="arrow-right" class="w-5 ml-3" />
                </button>
            </div>
            <div className="-mr-40 -ml-24 -mb-6 pt-11 relative z-30">
                <img src="../assets/header-img.png" class="" alt="HeaderImg">
            </div>
        </div>
        <div class="absolute bottom-0 inset-x-0 bg-white p-28" />
    </div>
</template>
