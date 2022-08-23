<script>
import LearningResource from "./LearningResource.vue";

export default {
  components: { LearningResource },
  inject: ["resources"],
};
</script>

<template>
  <ul>
    <learning-resource
      v-for="resource in resources"
      :key="resource.id"
      :description="resource.description"
      :id="resource.id"
      :link="resource.link"
      :title="resource.title"
    ></learning-resource>
  </ul>
</template>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
