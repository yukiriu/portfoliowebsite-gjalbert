<template>
  <div
    class="rounded-xl h-96 flex flex-col justify-between w-72 bg-gradient-to-b from-white to-gray-500 overflow-hidden text-black"
  >
    <div class="text-4xl m-2 ml-5 font-semibold">{{ name }}</div>
    <div class="text-lg my-2 mx-5">{{ desc }}</div>
    <div class="text-lg my-2 mx-5">{{ technologies }}</div>
    <div class="flex flex-row justify-around mb-10 w-3/4 mx-auto">
      <svg
        class="h-12 w-12"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
        />
      </svg>
      <a :href="gitHubLink">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          class="w-12 h-12"
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
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    desc: String,
    technologies: String,
    gitHubLink: String,
  },
};
</script>
<style scoped>
#background {
  filter: blur(4px);
}
</style>