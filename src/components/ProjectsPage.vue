<template>
  <div
    id="projectsPage"
    class="h-screen bg-gradient-to-r from-green-600 to-green-800 flex flex-row justify-evenly items-center"
  >
    <!-- <div class="flex flex-col absolute h-full">
            <marquee class="roboto text-white text-opacity-50 font-bold overflow-hidden w-full h-1/2"
                style="font-size: 20rem;"> PROJECTS. PROJECTS. PROJECTS. PROJECTS. PROJECTS. </marquee>
            <marquee direction="right" hspace="0"class="roboto text-white text-opacity-50 font-bold overflow-hidden w-full h-1/2"
                style="font-size: 20rem; top: 100;"> PROJECTS. PROJECTS. PROJECTS. PROJECTS. PROJECTS.  </marquee>
        </div> -->
      <div v-for="project in projects" :key="project.name" class="">
        <ProjectV2
          :name="project.name"
          :desc="project.desc"
          :technologies="project.technologies"
          :gitHubLink="project.gitHubLink"
          :image="project.image"
        ></ProjectV2>
      </div>
    </div>
</template>
<script>
import ProjectV2 from "./Project.vue";

export default {
  components: {
    ProjectV2
  },
  data() {
    return {
      projects: [
        {
          name: "Yukolors",
          desc: "Coolors clone to familiarize myself with Vue.Js and Laravel",
          technologies: "HTML, CSS, JavaScript, Vue.js, Laravel, TailwindCSS",
          gitHubLink: "https://github.com/yukiriu/yukolors",
          image: "/img/Yukolors.93e06577.svg"

        },
        {
          name: "Personal website",
          desc: "Personal website to showcase projects and skills",
          technologies: "HTML, CSS, Vue.js, JavaScript",
          gitHubLink: "https://github.com/yukiriu/portfoliowebsite-gjalbert",
          image: "/img/portfoliowebsite-gjalbert.b108079f.svg"
        }
      ],
    };
  },
};
</script>

