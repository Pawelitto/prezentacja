<script setup>
import { initFlowbite } from 'flowbite'

const props = defineProps({
    data: Object,
})

onMounted(() => {
    initFlowbite();
})
</script>
<template>
    <article class="p-4 mx-auto max-w-sm bg-white rounded-lg shadow-md border border-gray-200 dark:border-gray-800 dark:bg-gray-800">
        <a href="#">
            <img class="h-[100px] max-w-[300px] object-cover mb-5 rounded-lg" :src="data.img" :alt="data.rodzaj" />
        </a>
        <h3 class="mb-2 text-xl font-bold tracking-tight text-gray-900 lg:text-2xl dark:text-white">
            <a href="#">{{ data.name }}</a>
        </h3>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Typ: </span>{{ data.typ }}</p>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Rodzaj: </span>{{ data.rodzaj_aplikacji }}</p>
        <p class="mb-3 text-gray-500 dark:text-gray-400"><span class="text-gray-900 dark:text-white font-bold">Opis: </span>{{ data.opis }}</p>

        <button :data-modal-target="data.name" :data-modal-toggle="data.name" class="inline-flex items-center font-medium text-primary-600 hover:text-primary-800 dark:text-primary-500 hover:no-underline" type="button">
            Czytaj więcej <svg class="mt-px ml-1 w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10"><path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/></svg> 
        </button>
    </article>
</template>