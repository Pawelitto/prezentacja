<script setup>


const frameworks = {
  "React": {
    "Typ": "Biblioteka front-end",
    "Rodzaj aplikacji": "Aplikacje webowe typu SPA (Single Page Applications)",
    "Opis": "React to popularna biblioteka stworzona przez Facebooka do budowy interfejsów użytkownika. Jest używana głównie do tworzenia dynamicznych, interaktywnych stron internetowych."
  },
  "Angular": {
    "Typ": "Framework front-end",
    "Rodzaj aplikacji": "Aplikacje webowe typu SPA i MPA (Multi-Page Applications)",
    "Opis": "Angular to kompleksowy framework rozwijany przez Google. Zapewnia narzędzia do tworzenia zarówno prostych stron internetowych, jak i skomplikowanych aplikacji enterprise."
  },
  "Node.js": {
    "Typ": "Środowisko back-end",
    "Rodzaj aplikacji": "Aplikacje serwerowe i mikroserwisy",
    "Opis": "Node.js to środowisko uruchomieniowe JavaScript po stronie serwera. Jest używane do tworzenia skalowalnych aplikacji serwerowych i API."
  },
  "Express.js": {
    "Typ": "Framework back-end",
    "Rodzaj aplikacji": "Aplikacje serwerowe i API",
    "Opis": "Express.js to minimalistyczny framework do tworzenia aplikacji serwerowych w Node.js. Jest często stosowany do tworzenia API RESTful."
  },
  "Vue.js": {
    "Typ": "Biblioteka front-end",
    "Rodzaj aplikacji": "Aplikacje webowe typu SPA",
    "Opis": "Vue.js to prosta i elastyczna biblioteka do budowy interfejsów użytkownika. Jest często wybierana przez deweloperów do mniejszych projektów."
  },
  "Ember.js": {
    "Typ": "Framework front-end",
    "Rodzaj aplikacji": "Aplikacje webowe typu SPA",
    "Opis": "Ember.js to framework front-end, który dostarcza zestaw konwencji i narzędzi do tworzenia skomplikowanych aplikacji webowych."
  },
  "Meteor": {
    "Typ": "Framework full-stack",
    "Rodzaj aplikacji": "Aplikacje webowe typu SPA i MPA",
    "Opis": "Meteor to framework full-stack, który obsługuje zarówno front-end, jak i back-end. Umożliwia tworzenie czasu rzeczywistego (real-time) aplikacji webowych."
  },
  "Electron": {
    "Typ": "Framework do tworzenia aplikacji desktopowych",
    "Rodzaj aplikacji": "Aplikacje desktopowe",
    "Opis": "Electron pozwala na tworzenie aplikacji desktopowych przy użyciu HTML, CSS i JavaScript. Jest używany do budowy aplikacji na różne platformy, takie jak Windows, macOS i Linux."
  },
  "D3.js": {
    "Typ": "Biblioteka front-end",
    "Rodzaj aplikacji": "Wizualizacje danych i grafiki interaktywne",
    "Opis": "D3.js to biblioteka służąca do tworzenia interaktywnych wizualizacji danych w przeglądarkach internetowych."
  },
  "Nest.js": {
    "Typ": "Framework back-end",
    "Rodzaj aplikacji": "Aplikacje serwerowe i API",
    "Opis": "Nest.js to framework back-end oparty na TypeScript, który promuje strukturalne i skalowalne podejście do tworzenia aplikacji serwerowych."
  }
}

</script>
<template>
  <aside aria-label="Related articles" class="py-8 bg-white dark:bg-gray-900 lg:py-16 antialiased" />
  <div class="px-4 mx-auto w-full max-w-screen-xl">
      <h2 class="mb-8 text-2xl font-bold text-gray-900 dark:text-white">Trending on Flowbite</h2>
      <div id="animation-carousel" data-carousel="slide">
          <div class="relative overflow-hidden rounded-lg h-[600px]">
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">
                      
                  </div>
              </div>
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">

                  </div>
              </div>
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">

                  </div>
              </div>
          </div>
          <div class="flex justify-center items-center mt-4">
              <button type="button" class="flex justify-center items-center mr-4 h-full cursor-pointer group focus:outline-none" data-carousel-prev>
                  <span class="text-gray-500 dark:text-gray-400 hover:text-gray-700 dark:hover:text-gray-200">
                      <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10"><path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 5H1m0 0 4 4M1 5l4-4"/></svg>
                      <span class="hidden">Previous</span>
                  </span>
              </button>
              <button type="button" class="flex justify-center items-center h-full cursor-pointer group focus:outline-none" data-carousel-next>
                  <span class="text-gray-500 dark:text-gray-400 hover:text-gray-700 dark:hover:text-gray-200">
                      <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10"><path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/></svg> 
                      <span class="hidden">Next</span>
                  </span>
              </button>
          </div>
      </div>
  </div>
</template>