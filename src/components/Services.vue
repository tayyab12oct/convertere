<template>
    <div class="relative -mt-38 md:pt-40 pt-32 z-20">
        <img src="../assets/blue-bg.png" class="absolute inset-0 w-full h-full" alt="Gradient" />
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
                        class="font-bold text-primary-100 lg:px-5.5 px-3 lg:-mx-5.5 -mx-3 pt-12 mb-4 lg:leading-2 md:leading-6 leading-2 lg:text-2xl md:text-xl text-lg border-b-[20px] border-secondary-600">
                        {{v.title}}</p>
                    <p class="text-sm text-primary-100">{{v.desc}}</p>
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
        title: "Dla sportowców",
        desc: "To bardzo ważne by dobrze przygotować organizm do wysiłku, sesje w komorze normobarycznej sprzyjają poprawie jakości snu, to ważne by szybciej zasypiać i nie budzić się w ciągu nocy. Dobry sen jest gwarancją dobrego zdrowia i pełnej sprawności ponadto lepsze dotlenienie sprzyja zwiększeniu wydolności organizmu. Pobyt w komorze sprzyja szybszej regeneracji po zawodach. To czas relaksu gdzie można skupić się tylko na sobie odizolować się od zgiełku otaczającego nas świata."
    },
    {
        src: card2,
        imgClass: "lg:w-22 w-14",
        title: "Dla chorych",
        desc: "Powikłania pochorobowe mogą odebrać nam sprawność i komfort życia. Sesje tlenowe mają istotny wpływ na poprawę samopoczucia i oddychania. Pobyt w komorze to także szybsze gojenie się ran (np. po ciężkich oparzeniach, pooperacyjnych), co ważne bez konieczności zdejmowania opatrunków. Tlenoterapia w komorze daje niesamowite efekty w leczeniu tzw. stopy cukrzycowej, problemów dermatologicznych,  kardiologicznych , onkologicznych i wielu, wielu innych."
    },
    {
        src: card3,
        imgClass: "lg:w-16 w-12",
        title: "Dla dzieci i seniorów",
        desc: "Badania dowiodły, że terapia tlenowa jest ogromnym wsparciem w zaburzeniach wywołanych autyzmem, adhd.  Dorosłym i zabieganym daje ukojenie, wycisza, relaksuje, pomaga walczyć z nadwagą, depresją, a dla seniorów jest nieocenionym wsparciem w eliminacji stanów zapalnych, ogranicza dolegliwości bólowe (np. reumatycznych). Wyraźnie zmniejsza zaburzenia wywołane chorobą Alzheimera."
    },
]
</script>
