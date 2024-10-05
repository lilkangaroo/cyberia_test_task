<template>
  <div class="project_cat" v-for="item in project_categories" :key="item">
    <button v-for="category in item" :key="category">
      {{ category.name }}
    </button>
  </div>
</template>
<script>
import axios from "axios";

export default {
  data() {
    return {
      project_categories: [],
    };
  },
  methods: {
    async fetchCategories() {
      try {
        const response = await axios.get(
          "https://api.test.cyberia.studio/api/v1/project-categories"
        );
        this.project_categories = response.data;
      } catch (e) {
        alert("Ошибка загрузки категорий проекта");
      }
    },
  },
  mounted() {
    this.fetchCategories();
  },
};
</script>
<style></style>
