<script setup>

const props = defineProps({
    typ: String,
    opis: String,
    img: String,
    rodzaj: String,
})

</script>
<template>
    <article class="p-4 mx-auto max-w-sm bg-white rounded-lg shadow-md border border-gray-200 dark:border-gray-800 dark:bg-gray-800 dark:border-gray-700">
        <a href="#">
            <img class="mb-5 rounded-lg" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/blog/office-laptops.png" alt="office laptop working">
        </a>
        <h3 class="mb-2 text-xl font-bold tracking-tight text-gray-900 lg:text-2xl dark:text-white">
            <a href="#">React</a>
        </h3>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Typ: </span>Biblioteka front-end</p>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Rodzaj: </span>Aplikacje webowe typu SPA (Single Page Applications)</p>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Opis: </span>React to popularna biblioteka stworzona przez Facebooka do budowy interfejsów użytkownika. Jest używana głównie do tworzenia dynamicznych, interaktywnych stron internetowych.</p>
        <a href="#" class="inline-flex items-center font-medium text-primary-600 hover:text-primary-800 dark:text-primary-500 hover:no-underline">
            Czytaj więcej <svg class="mt-px ml-1 w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10"><path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/></svg> 
        </a>
    </article>
</template>