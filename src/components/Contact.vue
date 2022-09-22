<template>
    <div class="relative">
        <img src="../assets/contact.png" alt="circle" class="hidden xl:block absolute right-0 w-44 top-64 translate-y-1/2" />
        <div class="lg:px-12 px-5 md:py-20 py-16 max-w-6xl w-full mx-auto relative">
            <h1 class="text-secondary-400 md:text-6xl text-5xl tracking-wide text-center font-bold">Kontakt</h1>
            <p class="text-center text-gray-600 md:text-xl text-base max-w-4xl md:p-8 mx-auto pt-5">Lorem ipsum dolor
                sit
                amet
                consectetur
                adipisicing elit. Atque quibusdam facere possimus illo
                dolores natus quo delectus! Iusto sunt.
            </p>
            <div class="grid md:grid-cols-2 lg:gap-20 md:gap-10 gap-14 pt-14 pb-12">
                <div class="">
                    <h3 class="text-primary-100 md:text-xl text-base font-bold">Mapa dojazdu</h3>
                    <div class="h-72 w-full bg-gray-100 md:mt-10 my-6 md:mb-12"></div>
                    <h3 class="text-primary-100 md:text-xl text-base font-bold py-1.5">Adres</h3>
                    <p class="text-gray-600 md:text-lg text-base">Convertere Normobaria <br>ul. Pszczyńska 61 <br>
                        44-240 Żory
                    </p>
                    <p class="text-gray-600 md:text-lg text-base mt-2">+48 666 166 646</p>
                    <a href="mailto:biuro@convertere.pl"
                        class="text-primary-100 md:text-lg text-base font-semibold underline">biuro@convertere.pl</a>
                </div>
                <div class="space-y-5">
                    <h3 class="text-primary-100 md:text-xl text-base font-bold">Napisz do nas</h3>
                    <p class="text-gray-600 md:text-xl text-base pr-3">Lorem ipsum dolor sit amet, consectet Lorem ipsum
                        dolor
                        sit amet,
                        consectet
                    </p>
                    <input placeholder="Lorem ipsum dolor sit amet" type="text"
                        class="w-full md:text-lg text-base px-4 bg-white placeholder-gray-150 border-2 border-gray-150 focus:outline-none py-3" />
                    <input placeholder="Ipsum dolor sit amet" type="email"
                        class="w-full md:text-lg text-base px-4 bg-white placeholder-gray-150 border-2 border-gray-150 focus:outline-none py-3" />
                    <textarea rows="8"
                        class="w-full md:text-lg text-base px-4 bg-white placeholder-gray-150 border-2 border-gray-150 focus:outline-none py-3"></textarea>
                    <button
                        class="bg-secondary-100 w-full rounded-full p-4.5 uppercase md:text-xl text-base font-bold text-primary-100">
                        Wyślij wiadomość
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>