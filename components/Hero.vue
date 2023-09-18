<template> 
<section class="bg-[url('https://store.hp.com/app/assets/images/uploads/prod/top-emerging-technologies-2019-hero1570216187790543.jpg')] bg-no-repeat bg-cover bg-center bg-gray-700 bg-blend-multiply">
    <div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-6">
        <div class="mx-auto max-w-screen-md text-center mb-8 lg:mb-12">
            <h2 class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white">Biblioteka a Framework</h2>
            <p class="mb-5 font-light text-gray-500 sm:text-xl dark:text-gray-400">Biblioteka i Framework to dwa różne podejścia do tworzenia oprogramowania w języku JavaScript (JS).</p>
        </div>
        <div class="space-y-8 lg:grid lg:grid-cols-2 sm:gap-6 xl:gap-10 lg:space-y-0">
            <!-- Pricing Card -->
            <div class="flex flex-col p-6 mx-auto max-w-lg text-center text-gray-900 bg-white rounded-lg border border-gray-100 shadow dark:border-gray-600 xl:p-8 dark:bg-gray-800 dark:text-white">
                <h2 class="mb-4 text-3xl font-semibold">Biblioteka</h2>
                <!-- <p class="font-light text-gray-500 sm:text-lg dark:text-gray-400">Definicja</p> -->
                <!-- <div class="flex justify-center items-baseline my-8">
                    <span class="mr-2 text-5xl font-extrabold">$29</span>
                    <span class="text-gray-500 dark:text-gray-400">/month</span>
                </div> -->
                <!-- List -->

                <ul class="space-y-4 text-gray-500 list-disc list-inside dark:text-gray-400">
                    Definicja:
                    <ol class="pl-5 mt-2 space-y-1 list-decimal list-inside text-left">
                        <li class="p-2">Biblioteka w JS to zbiór gotowych funkcji, narzędzi i komponentów, które mogą być używane w celu ułatwienia tworzenia aplikacji.</li>
                        <li class="p-2">Biblioteki są zwykle bardziej skoncentrowane na rozwiązaniu określonych zadań lub problemów, na przykład manipulacji DOM, zarządzaniu stanem lub obsłudze zapytań sieciowych.</li>
                        <li class="p-2">Biblioteki są zazwyczaj bardziej elastyczne i pozwalają programiście na wybór, kiedy i jak używać ich funkcji.</li>
                    </ol>
                </ul>


                <h3 class="mt-4 text-gray-500 sm:text-lg dark:text-white font-bold">Zalety</h3>
                <ul role="list" class="mb-8 space-y-4 text-left m-6">
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Bardziej elastyczne: </span>Pozwalają na wybór, które części biblioteki użyć w projekcie</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Lekkość: </span>Zazwyczaj są mniejsze w rozmiarze niż pełne frameworki, co może przyspieszyć ładowanie strony.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Dostępność specjalistycznych narzędzi: </span>Często oferują specjalistyczne funkcje i narzędzia, które można użyć w konkretnych przypadkach.</span>
                    </li>
                    
                </ul>

                <h3 class="mt-4 text-gray-500 sm:text-lg dark:text-white font-bold">Wady</h3>
                <ul role="list" class="mb-8 space-y-4 text-left m-6">
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Konieczność samodzielnego zarządzania: </span>Korzystając z bibliotek, programiści są bardziej odpowiedzialni za organizację i zarządzanie kodem. To może prowadzić do większej złożoności projektu, zwłaszcza w dużych aplikacjach.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Brak kompleksowych rozwiązań: </span>Biblioteki często nie oferują kompleksowych rozwiązań do zarządzania stanem lub routowania, co oznacza, że programiści muszą korzystać z wielu różnych bibliotek lub pisać własne rozwiązania.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Wymaga większego zaangażowania programisty: </span>: Programista musi podejmować więcej decyzji dotyczących architektury projektu.</span>
                    </li>
                </ul>

            </div>
            <!-- Pricing Card -->
            <div class="flex flex-col p-6 mx-auto max-w-lg text-center text-gray-900 bg-white rounded-lg border border-gray-100 shadow dark:border-gray-600 xl:p-8 dark:bg-gray-800 dark:text-white">
                <h2 class="mb-4 text-3xl font-semibold">Framework</h2>
                <!-- <p class="font-light text-gray-500 sm:text-lg dark:text-gray-400">Definicja</p> -->
                <!-- <div class="flex justify-center items-baseline my-8">
                    <span class="mr-2 text-5xl font-extrabold">$29</span>
                    <span class="text-gray-500 dark:text-gray-400">/month</span>
                </div> -->
                <!-- List -->

                <ul class="space-y-4 text-gray-500 list-disc list-inside dark:text-gray-400">
                    Definicja:
                    <ol class="pl-5 mt-2 space-y-1 list-decimal list-inside text-left">
                        <li class="p-2">Framework to kompleksowy zestaw zasad, narzędzi i szablonów, które definiują strukturę i sposób budowy aplikacji.</li>
                        <li class="p-2">Frameworki narzucają pewne ograniczenia i konwencje, co może przyspieszyć proces tworzenia aplikacji, ale także ograniczyć elastyczność w pewnym stopniu.</li>
                        <li class="p-2">Frameworki często zapewniają gotowe rozwiązania do obsługi rutynowych zadań, takich jak zarządzanie stanem, routowanie, interakcje z bazą danych i wiele innych.</li>
                    </ol>
                </ul>


                <h3 class="mt-4 text-gray-500 sm:text-lg dark:text-white font-bold">Zalety</h3>
                <ul role="list" class="mb-8 space-y-4 text-left m-6">
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Struktura i konwencje: </span> Zapewniają jasną strukturę i konwencje, co ułatwia organizację projektu i współpracę w zespole.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Gotowe rozwiązania: </span>Często zawierają gotowe moduły do często wykorzystywanych zadań, co przyspiesza rozwijanie aplikacji.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="flex-shrink-0 w-5 h-5 text-green-500 dark:text-green-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Wsparcie społeczności: </span>Popularne frameworki mają duże społeczności, co oznacza dostęp do wielu przydatnych bibliotek i rozszerzeń.</span>
                    </li>
                    
                </ul>

                <h3 class="mt-4 text-gray-500 sm:text-lg dark:text-white font-bold">Wady</h3>
                <ul role="list" class="mb-8 space-y-4 text-left m-6">
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Mniej elastyczne: </span>Narzucają pewne ograniczenia, które mogą nie pasować do konkretnego projektu.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Wymaga nauki: </span> Programiści muszą nauczyć się używać konkretnego frameworka, co może wymagać pewnego czasu.</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <!-- Icon -->
                        <svg class="w-12 h-12 text-red-500" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7-6 6m0-6 6 6m6-3a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"/>
                        </svg>  
                        <span class="text-gray-900 dark:text-gray-400"><span class="dark:text-white dark-text-gray-700">Może być nadmiernie rozbudowane: </span> Niektóre frameworki są bardzo rozbudowane, co może prowadzić do nadmiernego skomplikowania w mniejszych projektach.</span>
                    </li>
                </ul>

            </div>
        </div>
    </div>
  </section>
</template>