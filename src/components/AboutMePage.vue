<template>
  <div
    id="aboutMePage"
    class="h-screen bg-gray-200 flex flex-col items-center justify-center m-auto overflow-hidden"
  >
    <div class="flex flex-row justify-around items-center w-3/5">
      <div
        class="w-72 h-72 rounded-xl bg-gradient-to-b from-green-600 to-green-800"
      >
        <div
          class="h-72 w-72 rounded-xl bg-green-300 -mt-6 ml-6 overflow-hidden"
        >
          <img src="../assets/125418887_390177505770517_9110273786534809879_n.jpg" />
        </div>
      </div>
      <div
        class="flex flex-col justify-center bg-green-600 px-10 pb-2 h-64 text-white rounded-xl bg-gradient-to-b from-green-600 to-green-800 font-semibold"
      >
        <div class="font-bold md:text-4xl lg:text-5xl sm:text-2xl h-auto">
          Gabriel Jalbert
        </div>
        <div class="flex items-center w-64 justify-start mb-1">
          <img class="w-8 h-8" src="../assets/GitHub-Mark-Light-32px.png" alt="" />
          <div class="ml-2">My GitHub</div>
        </div>
        <div class="flex items-center w-64 justify-start mb-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="h-8 w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"
            />
          </svg>
          <div class="ml-2">Resume</div>
        </div>
        <div class="flex items-center w-64 justify-start mb-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="h-8 w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
            />
          </svg>
          <div class="ml-2">gabrieljalbert@gjalbert.com</div>
        </div>
        <div class="flex items-center w-64 justify-start mb-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="h-8 w-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"
            />
          </svg>
          <div class="ml-2">438 520 7542</div>
        </div>
        <div class="flex items-center w-64 justify-start mb-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-8 h-8"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
            />
          </svg>
          <div class="ml-2">Boisbriand, Québec</div>
        </div>
      </div>
    </div>
    <div class="w-3/5 px-10">
      <div class="mt-10 text-4xl">About me!</div>
      <div class="h-1 w-full bg-green-600"></div>
      <div class="mt-2 text-lg text-justify">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Itaque
        necessitatibus explicabo illo impedit deserunt veritatis voluptate
        tenetur unde pariatur, reiciendis exercitationem, error eaque
        praesentium qui officiis quae ex ratione maiores. Lorem ipsum dolor sit
        amet consectetur adipisicing elit. Nulla libero voluptates
        exercitationem minima praesentium dolorem. In illum earum vero
        necessitatibus ducimus dignissimos, sunt, maiores aperiam inventore fuga
        nihil distinctio corporis.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutMePage",
  components: {},
};
</script>

<style scoped>
    #aboutMePage {
        background-image: url("../assets/dot-grid.png");
    }
</style>