<template>
<div class="bg-gray-500 rounded-xl h-48 w-96 transition-transform duration-200 project mx-6 my-10 sm:w-96 md:w-128 lg:w-128">
  <div
    class="bg-white h-48 w-96 items-start ml-4 absolute -mt-4 rounded-xl py-2 px-2 sm:py-4 sm:px-2 md:py-6 md:px-4 sm:w-96 md:w-128 lg:w-128"
  >
    <div class="flex flex-row justify-start h-full mx-1 h">
      <div class=" flex flex-col justify-evenly md:justify-between h-full">
        <a :href="hostedLink" target="_blank" v-if="hostedLink !== undefined">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-12 h-12 text-gray-400 hover:text-gray-600 duration-75"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
            />
          </svg>
        </a>
        <a :href="gitHubLink" target="_blank" >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-12 h-12 text-gray-400 hover:text-gray-600 duration-75"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"
            />
          </svg>
        </a>
      </div>
      <div class="flex flex-col justify-between ml-4">
        <div class="text-3xl font-semibold text-left">{{ name }}</div>
        <div class="">
          <div class="my-2 font-semibold pr-2 text-justify">{{ desc }}</div>
          <div class="mb-4 text-pink-800 font-semibold italic">{{ technologies }}</div>
        </div>
      </div>
    </div>
  </div>
</div>
  
</template>

<script>
export default {
  props: {
    name: String,
    desc: String,
    technologies: String,
    gitHubLink: String,
    hostedLink: String
  },
};
</script>

<style scoped>
  .project:hover {
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}
</style>