<template>
  <div
    id="projectsPage"
    class="h-screen bg-gradient-to-r from-green-600 to-green-800"
  >
    <!-- <div class="flex flex-col absolute h-full">
            <marquee class="roboto text-white text-opacity-50 font-bold overflow-hidden w-full h-1/2"
                style="font-size: 20rem;"> PROJECTS. PROJECTS. PROJECTS. PROJECTS. PROJECTS. </marquee>
            <marquee direction="right" hspace="0"class="roboto text-white text-opacity-50 font-bold overflow-hidden w-full h-1/2"
                style="font-size: 20rem; top: 100;"> PROJECTS. PROJECTS. PROJECTS. PROJECTS. PROJECTS.  </marquee>
        </div> -->
    <div v-for="project in projects" :key="project.name">
      <Project :name = project.name :desc = project.desc :technologies= project.technologies :gitHubLink = project.gitHubLink ></Project>
    </div>
  </div>
</template>
<script>
import Project from "./Project.vue";
export default {
  components: {
    Project,
  },
  data() {
    return {
      projects: [{ name: "Yukolors", desc: "Simple coolors clone", technologies: "Vue.js, Laravel, TailwindCSS", gitHubLink: "https://github.com/yukiriu/yukolors",  }],
    };
  },
};
</script>