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
  <div :id="data.name" data-modal-backdrop="static" tabindex="-1" aria-hidden="true" class="fixed top-0 left-0 right-0 z-50 hidden w-full p-4 overflow-x-hidden overflow-y-auto md:inset-0 h-[calc(100%-1rem)] max-h-full">
      <div class="relative w-full max-w-2xl max-h-full">
          <!-- Modal content -->
          <div class="relative bg-white rounded-lg shadow dark:bg-gray-700">
              <!-- Modal header -->
              <div class="flex items-start justify-between p-4 border-b rounded-t dark:border-gray-600">
                    <NuxtLink :to="data.link" target="_blank"> 
                      <div class="content">
                        <h2>{{ data.name }}</h2>
                        <h2>{{ data.name }}</h2>
                      </div>
                    </NuxtLink>
                  <button type="button" class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ml-auto mr-5 inline-flex justify-center items-center " :data-modal-hide="data.name">
                    <NuxtLink :to="data.link" target="_blank">
                    <img class="h-[100px] max-w-[300px] object-cover mb-5 rounded-lg dark:hover:bg-gray-600 dark:hover:text-white" :src="data.img" :alt="data.rodzaj" />
                      <span class="sr-only">Close modal</span>
                    </NuxtLink>
                  </button>
              </div>
              <!-- Modal body -->
              <div class="p-6 space-y-6">
                  <p class="text-base leading-relaxed text-gray-500 dark:text-gray-400">
                      {{ data.tech }}
                  </p>
              </div>
              <!-- Modal footer -->
              <div class="flex items-center p-6 space-x-2 border-t border-gray-200 rounded-b dark:border-gray-600">
                  <button :data-modal-hide="data.name" type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Rozumiem :)</button>
              </div>
          </div>
      </div>
  </div>
</template>
<style scoped>
.content {
  position: relative;
}

.content h2 {
  color: #fff;
  font-size: 3em;
  position: absolute;
  top: -10px;
}

.content h2:nth-child(1) {
  color: transparent;
  -webkit-text-stroke: 1px #fff;
}

.content h2:nth-child(2) {
  color: #fff;
  animation: animate 4s ease-in-out infinite;
}

@keyframes animate {
  0%,
  100% {
    clip-path: polygon(
      0% 45%,
      16% 44%,
      33% 50%,
      54% 60%,
      70% 61%,
      84% 59%,
      100% 52%,
      100% 100%,
      0% 100%
    );
  }

  50% {
    clip-path: polygon(
      0% 60%,
      15% 65%,
      34% 66%,
      51% 62%,
      67% 50%,
      84% 45%,
      100% 46%,
      100% 100%,
      0% 100%
    );
  }
}
</style>