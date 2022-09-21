<template>
    <div class="relative">
        <img src="../assets/newsletter.jpeg" class="absolute inset-0 w-full h-full" alt="Newsletter">
        <div
            className="relative md:px-12 px-5 lg:py-22 md:py-12 py-10 max-w-6xl w-full mx-auto flex lg:flex-row flex-col items-center justify-between lg:space-x-10 md:space-x-2">
            <p className="text-white lg:text-4xl md:text-3xl text-2xl tracking-wide font-bold">
                Zapisz się na Newsletter!
            </p>
            <div className="mt-6 lg:mt-0 md:flex-1 bg-white p-1 rounded-full w-full max-w-lg">
                <form className="flex w-full md:w-auto">
                    <input placeholder="Wpisz Twój email" type="email" name="email"
                        class="w-full lg:text-lg md:text-base text-sm px-4 bg-transparent placeholder-gray-150 focus:outline-none py-3 rounded-full" />
                    <button type="submit"
                        className="flex items-center justify-center rounded-full whitespace-nowrap border border-transparent bg-primary-100 px-5 py-3 tracking-wide lg:text-lg md:text-base text-sm uppercase font-bold text-secondary-400 focus:outline-none">
                        Zapisz się >
                    </button>
                </form>
            </div>
        </div>
    </div>
</template>