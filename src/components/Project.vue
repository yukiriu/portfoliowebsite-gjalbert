<template>
  <div
    class="bg-white border border-gray-300 shadow rounded-md p-4 w-128 mx-auto h-auto"
  >
    <div class="flex space-x-4">
      <div class="h-8 w-8 text-gray-400">
        <a :href="gitHubLink">
          <svg
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
        </a>
      </div>
      <div class="flex-1 space-y-4 py-1">
        <div class="">{{ name }}</div>
        <div class="space-y-2">
          <div class="h-4 bg-gray-400 rounded"></div>
          <div class="h-4 bg-gray-400 rounded w-5/6"></div>
          <div>{{ desc }}</div>
          <div>{{ technologies }}</div>
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
  },
};
</script>