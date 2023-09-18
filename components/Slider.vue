<script setup>

const frameworks = [
  {
    name: "React",
    img: "https://cdn1.iconfinder.com/data/icons/programing-development-8/24/react_logo-512.png",
    typ: "Biblioteka front-end",
    tech: "React to potężna biblioteka JavaScript stworzona przez Facebooka, która rewolucjonizuje sposób, w jaki buduje się interfejsy użytkownika. Opiera się na komponencjach, co sprawia, że kod jest modułowy i łatwy do zarządzania. React używa wirtualnego DOM, co przyspiesza wydajność aplikacji poprzez minimalizację zmian w rzeczywistym DOM. Jedną z jego głównych zalet jest jednokierunkowy przepływ danych, co ułatwia zarządzanie stanem aplikacji. Dodatkowo, ogromna społeczność oraz wiele dostępnych narzędzi i bibliotek sprawiają, że React jest świetnym wyborem do budowy nowoczesnych aplikacji webowych.",
    link: "https://react.dev/",
    rodzaj_aplikacji: "Aplikacje webowe typu SPA (Single Page Applications)",
    opis: "React to popularna biblioteka stworzona przez Facebooka do budowy interfejsów użytkownika. Jest używana głównie do tworzenia dynamicznych, interaktywnych stron internetowych."
  },
  {
    name: "Angular",
    img: "https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/Angular_full_color_logo.svg/512px-Angular_full_color_logo.svg.png",
    typ: "Framework front-end",
    tech: "Angular, stworzony przez Google, to framework front-end, który oferuje pełne narzędzia do tworzenia skalowalnych i modułowych aplikacji webowych. Jest oparty na TypeScript, co pozwala na bardziej typową i bezpieczną pracę z kodem JavaScript. Angular wprowadza koncepcję dwukierunkowego wiązania danych, co oznacza, że zmiany w widoku automatycznie aktualizują dane w modelu i na odwrót. Ponadto, framework dostarcza wiele gotowych rozwiązań, takich jak moduły, routing czy obsługa formularzy, co przyspiesza proces tworzenia aplikacji.",
    link: "https://angular.io/",
    rodzaj_aplikacji: "Aplikacje webowe typu SPA i MPA (Multi-Page Applications)",
    opis: "Angular to kompleksowy framework rozwijany przez Google. Zapewnia narzędzia do tworzenia zarówno prostych stron internetowych, jak i skomplikowanych aplikacji enterprise."
  },
  {
    name: "Node.js",
    img: "https://upload.vectorlogo.zone/logos/nodejs/images/7bd728ca-9a92-4137-9792-dfb1b41b8ce7.svg",
    typ: "Środowisko back-end",
    tech: "Node.js to środowisko uruchomieniowe JavaScript po stronie serwera, które umożliwia tworzenie skalowalnych i wydajnych aplikacji serwerowych. Jego asynchroniczna natura sprawia, że jest idealny do obsługi wielu równoczesnych żądań. Node.js używa silnika V8, co przekłada się na wydajność i szybkość. Możliwość tworzenia mikroserwisów i serwerów API czyni go popularnym wyborem dla aplikacji backendowych.",
    link: "https://nodejs.org/en",
    rodzaj_aplikacji: "Aplikacje serwerowe i mikroserwisy",
    opis: "Node.js to środowisko uruchomieniowe JavaScript po stronie serwera. Jest używane do tworzenia skalowalnych aplikacji serwerowych i API."
  },
  {
    name: "Express.js",
    img: "https://www.vectorlogo.zone/logos/expressjs/expressjs-ar21.png",
    typ: "Framework back-end",
    tech: "Express.js to minimalistyczny framework do tworzenia aplikacji serwerowych w Node.js. Jego prostota pozwala na szybkie tworzenie API RESTful i serwerów internetowych. Express oferuje wiele gotowych rozwiązań, takich jak middleware, obsługa trasowania i obsługa zapytań HTTP, co znacznie przyspiesza rozwijanie serwerów Node.js.",
    link: "https://expressjs.com/",
    rodzaj_aplikacji: "Aplikacje serwerowe i API",
    opis: "Express.js to minimalistyczny framework do tworzenia aplikacji serwerowych w Node.js. Jest często stosowany do tworzenia API RESTful."
  },
  {
    name: "Vue.js",
    img: "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/555px-Vue.js_Logo_2.svg.png",
    typ: "Biblioteka front-end",
    tech: "Vue.js to lekka i elastyczna biblioteka do budowy interfejsów użytkownika. Jego prosty składniowy szablon i jednokierunkowy przepływ danych ułatwiają tworzenie interaktywnych komponentów. Vue.js integruje się dobrze z innymi projektami i może być stopniowo wprowadzany do istniejących aplikacji. To świetny wybór dla mniejszych projektów, które wymagają dynamicznego interfejsu użytkownika.",
    link: "https://vuejs.org/",
    rodzaj_aplikacji: "Aplikacje webowe typu SPA",
    opis: "Vue.js to prosta i elastyczna biblioteka do budowy interfejsów użytkownika. Jest często wybierana przez deweloperów do mniejszych projektów."
  },
  {
    name: "Ember.js",
    img: "https://emberjs.com/images/brand/ember-4c.svg",
    typ: "Framework front-end",
    tech: "Ember.js to kompleksowy framework front-end, który dostarcza zestaw konwencji i narzędzi do tworzenia skomplikowanych aplikacji webowych. Jego architektura opiera się na wzorcu MVC (Model-View-Controller), co pomaga w organizacji kodu. Ember.js oferuje wiele narzędzi do automatyzacji procesu budowy, testowania i wdrażania aplikacji.",
    link: "https://emberjs.com/",
    rodzaj_aplikacji: "Aplikacje webowe typu SPA",
    opis: "Ember.js to framework front-end, który dostarcza zestaw konwencji i narzędzi do tworzenia skomplikowanych aplikacji webowych."
  },
  {
    name: "Meteor",
    img: "https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/meteor-js-icon.png",
    typ: "Framework full-stack",
    tech: "Meteor to framework full-stack, który umożliwia tworzenie aplikacji zarówno po stronie klienta, jak i serwera, przy użyciu jednego języka - JavaScript. Jest idealny do tworzenia czasu rzeczywistego (real-time) aplikacji webowych, takich jak czaty czy aplikacje społecznościowe. Meteor oferuje wbudowane funkcje, takie jak synchronizacja danych, co ułatwia rozwijanie interaktywnych aplikacji.",
    link: "https://www.meteor.com/",
    rodzaj_aplikacji: "Aplikacje webowe typu SPA i MPA",
    opis: "Meteor to framework full-stack, który obsługuje zarówno front-end, jak i back-end. Umożliwia tworzenie czasu rzeczywistego (real-time) aplikacji webowych."
  },
  {
    name: "Electron",
    img: "https://cdn.icon-icons.com/icons2/2699/PNG/512/electronjs_logo_icon_168222.png",
    typ: "Framework do tworzenia aplikacji desktopowych",
    tech: "Electron to framework do tworzenia aplikacji desktopowych przy użyciu webowych technologii, takich jak HTML, CSS i JavaScript. Pozwala na tworzenie aplikacji na różne platformy, co jest szczególnie przydatne dla deweloperów tworzących narzędzia desktopowe i aplikacje biurkowe.",
    link: "https://www.electronjs.org/",
    rodzaj_aplikacji: "Aplikacje desktopowe",
    opis: "Electron pozwala na tworzenie aplikacji desktopowych przy użyciu HTML, CSS i JavaScript. Jest używany do budowy aplikacji na różne platformy, takie jak Windows, macOS i Linux."
  },
  {
    name: "D3.js",
    img: "https://raw.githubusercontent.com/d3/d3-logo/master/d3.png",
    typ: "Biblioteka front-end",
    tech: "D3.js to zaawansowana biblioteka służąca do tworzenia interaktywnych wizualizacji danych w przeglądarkach internetowych. Pozwala na tworzenie różnorodnych grafik i wykresów, a także interakcji z nimi. D3.js daje pełną kontrolę nad wyglądem i zachowaniem wizualizacji.",
    link: "https://d3js.org/",
    rodzaj_aplikacji: "Wizualizacje danych i grafiki interaktywne",
    opis: "D3.js to biblioteka służąca do tworzenia interaktywnych wizualizacji danych w przeglądarkach internetowych."
  },
  {
    name: "Nest.js",
    img: "https://upload.wikimedia.org/wikipedia/commons/a/a8/NestJS.svg",
    typ: "Framework back-end",
    tech: "Nest.js to framework back-end oparty na TypeScript, który promuje strukturalne i skalowalne podejście do tworzenia aplikacji serwerowych. Wykorzystuje dekoratory i moduły, co pomaga w organizacji kodu i ułatwia testowanie aplikacji. Jest idealnym wyborem dla projektów wymagających solidnego backendu.",
    link: "https://nestjs.com/",
    rodzaj_aplikacji: "Aplikacje serwerowe i API",
    opis: "Nest.js to framework back-end oparty na TypeScript, który promuje strukturalne i skalowalne podejście do tworzenia aplikacji serwerowych."
  }
]

</script>
<template>
  <Modal v-for="framework in frameworks" :key="framework.name" :data="framework" />

  <aside aria-label="Related articles" class="py-8 bg-white dark:bg-gray-900 lg:py-16 antialiased" />
  <div class="px-4 mx-auto w-full max-w-screen-xl">
      <h2 class="mb-8 text-2xl font-bold text-gray-900 dark:text-white">Wybrane technologie</h2>
      <div id="animation-carousel" data-carousel="slide">
          <div class="relative overflow-hidden rounded-lg h-[450px]">
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">
                      <Artykul v-for="framework in frameworks.slice(0,3)" :key="framework.name" :data="framework" />
                  </div>
              </div>
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">
                    <Artykul v-for="framework in frameworks.slice(3,6)" :key="framework.name" :data="framework" />
                  </div>
              </div>
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">
                    <Artykul v-for="framework in frameworks.slice(6,9)" :key="framework.name" :data="framework" />
                  </div>
              </div>
              <div class="hidden bg-white duration-700 ease-in-out dark:bg-gray-900" data-carousel-item>
                  <div class="grid grid-cols-1 gap-4 sm:grid-cols-2 xl:grid-cols-3">
                    <Artykul v-for="framework in frameworks.slice(9, 10)" :key="framework.name" :data="framework" />
                  </div>
              </div>
              
          </div>
          <div class="flex justify-center items-center mt-4 pb-8">
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