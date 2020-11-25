<template>
  <div
    id="projectsPage"
    class="page  min-h-screen h-auto bg-gradient-to-r from-green-600 to-green-800 flex flex-col justify-center items-center"
  >
  <div class="text-8xl text-white workSans font-bold text-opacity-75">
    PROJETS
  </div>
    <div class="flex flex-row justify-evenly items-center w-4/5 h-auto flex-wrap m-10">
      <div v-for="project in projectsFR" :key="project.name" class="">
        <Project
          :name="project.name"
          :desc="project.desc"
          :technologies="project.technologies"
          :gitHubLink="project.gitHubLink"
          :hostedLink="project.hostedLink"
        ></Project>
      </div>
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
      projectsFR: [
        {
          name: "Yukolors",
          desc: "Recréation du site Coolors pour me familiariser avec Vue.Js et Laravel.",
          technologies: "HTML, CSS, TailwindCSS, Vue.js, JavaScript, Laravel",
          gitHubLink: "https://github.com/yukiriu/yukolors"
        },
        {
          name: "Site web personnel",
          desc: "Site web personnel pour mettre en valeur mes projets et habiletés.",
          technologies: "HTML, CSS, TailwindCSS Vue.js, JavaScript",
          gitHubLink: "https://github.com/yukiriu/portfoliowebsite-gjalbert",
          hostedLink: "https://gjalbert.com",
        },
        {
          name: "Site web pour Decked Out",
          desc:
            "Site web pour le jeu Decked Out, mon projet de fin de technique.",
          technologies: "HTML, CSS, TailwindCSS, JavaScript",
          gitHubLink: "https://github.com/yukiriu/deckedout-website",
          hostedLink: "https://flamboyant-poitras-1dab3b.netlify.app/",
        }
      ],
      projectsEN: [
        {
          name: "Yukolors",
          desc: "Coolors clone to familiarize myself with Vue.Js and Laravel",
          technologies: "HTML, CSS, TailwindCSS, Vue.js, JavaScript, Laravel",
          gitHubLink: "https://github.com/yukiriu/yukolors"
        },
        {
          name: "Personal website",
          desc: "Personal website to showcase projects and skills",
          technologies: "HTML, CSS, TailwindCSS Vue.js, JavaScript",
          gitHubLink: "https://github.com/yukiriu/portfoliowebsite-gjalbert",
          hostedLink: "/img/portfoliowebsite-gjalbert.b108079f.svg",
        },
        {
          name: "Decked Out website",
          desc:
            "Website to showcase Decked Out, a videogame we made as a team for our final year project",
          technologies: "HTML, CSS, TailwindCSS, JavaScript",
          gitHubLink: "https://github.com/yukiriu/deckedout-website",
          hostedLink: "https://flamboyant-poitras-1dab3b.netlify.app/",
        }
      ],
    };
  },
};
</script>

