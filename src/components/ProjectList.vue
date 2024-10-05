<template>
  <section>
    <h1>Кейсы</h1>
    <ProjectCategories />
    <TheProject
      class="project"
      v-for="project in projects"
      :key="project"
      :project="project"
    />
  </section>
</template>

<script>
import TheProject from "./TheProject.vue";
import ProjectCategories from "./ProjectCategories.vue";

export default {
  components: { TheProject, ProjectCategories },
  props: {
    projects: {
      type: Array,
      Required: true,
    },
  },
};
</script>

<style></style>
