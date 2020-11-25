<template>
  <div class="scrollContainer">
    <LandingPage></LandingPage>
    <AboutMePage></AboutMePage>
    <ProjectsPage></ProjectsPage>
  </div>
</template>

<script>
import LandingPage from "./LandingPage.vue";
import AboutMePage from "./AboutMePage.vue";
import ProjectsPage from "./ProjectsPage.vue";

export default {
  name: "Site",
  components: {
    LandingPage,
    AboutMePage,
    ProjectsPage,
  },
  
};


</script>