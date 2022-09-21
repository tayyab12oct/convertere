<template>
  <Popover class="bg-white shadow-md sticky top-0 z-40">
    <div class="md:px-12 px-5 md:py-6 py-4 max-w-6xl w-full mx-auto flex items-center justify-between">
      <div class="flex justify-start lg:w-0 lg:flex-1">
        <img src="../assets/logo.png" class="lg:h-12 h-9" alt="Logo" />
      </div>
      <div class="md:hidden">
        <PopoverButton
          class="inline-flex items-center justify-center rounded-md p-2 text-primary-100 bg-gray-100 focus:outline-none">
          <span class="sr-only">Open menu</span>
          <Bars3Icon class="h-6 w-6" aria-hidden="true" />
        </PopoverButton>
      </div>
      <PopoverGroup as="nav" class="hidden lg:space-x-10 space-x-8 md:flex">
        <a v-for="v in navs" :key="v" :href="v.href"
          class="lg:text-lg md:text-base font-bold text-primary-100 border-b-2 border-transparent focus:border-secondary-100 transition-all hover:border-secondary-100">
          {{v.name}}
        </a>
      </PopoverGroup>
    </div>

    <transition enter-active-class="duration-200 ease-out" enter-from-class="opacity-0 scale-95"
      enter-to-class="opacity-100 scale-100" leave-active-class="duration-100 ease-in"
      leave-from-class="opacity-100 scale-100" leave-to-class="opacity-0 scale-95">
      <PopoverPanel focus class="absolute inset-x-0 top-0 origin-top-right transform p-2 transition md:hidden">
        <div class="divide-y-2 divide-gray-50 rounded-lg bg-white shadow-lg ring-1 ring-black ring-opacity-5">
          <div class="p-5">
            <div class="flex items-center justify-between">
              <div>
                <img src="../assets/logo.png" class="lg:h-12 h-9" alt="Logo" />
              </div>
              <div class="-mr-2">
                <PopoverButton
                  class="inline-flex items-center justify-center rounded-md p-2 text-primary-100 bg-gray-100 focus:outline-none">
                  <span class="sr-only">Close menu</span>
                  <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                </PopoverButton>
              </div>
            </div>
            <div class="mt-6">
              <nav class="flex flex-col gap-y-5">
                <a v-for="v in navs" :key="v" :href="v.href"
                  class="text-sm font-semibold text-primary-100 border-b-2 pb-1 border-transparent focus:border-secondary-100 transition-all hover:border-secondary-100">
                  {{v.name}}
                </a>
              </nav>
            </div>
          </div>
        </div>
      </PopoverPanel>
    </transition>
  </Popover>
</template>

<script setup>
import {
  Popover,
  PopoverButton,
  PopoverGroup,
  PopoverPanel,
} from '@headlessui/vue'
import {
  Bars3Icon,
  XMarkIcon,
} from '@heroicons/vue/24/outline'

const navs = [
  {
    name: 'Korzyści',
    href: '#',
  },
  {
    name: 'Przygotowanie',
    href: '#',
  },
  {
    name: 'Cennik',
    href: '#',
  },
  {
    name: 'Kontakt',
    href: '#',
  },
]

</script>
