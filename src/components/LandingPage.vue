<template>
  <div
    class="page h-screen bg-gradient-to-b from-green-600 to-green-800 text-orange-100 workSans font-semibold text-6xl flex flex-col text-center items-center"
  >
    <div class="w-auto m-auto animate-fadeIn">
      <div class="-mb-3">GABRIEL</div>
      <div class="bg-orange-100 h-1"></div>
      <div class="-mt-3">JALBERT</div>
      <div class="text-sm workSans font-light">ÉTUDIANT EN INFORMATIQUE</div>
    </div>
    <div class="h-10 w-10 mb-10" v-on:click="scrollToPage('aboutMePage')">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        class="animate-bounce hover:opacity-50"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M19 9l-7 7-7-7"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  name: "LandingPage",
  components: {},
  methods: {
    scrollToPage(id) {
      document.getElementById(id).scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>