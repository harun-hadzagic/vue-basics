<template>
  <ul>
    <learning-resource
      v-for="resource in resources"
      :key="resource.id"
      :title="resource.title"
      :description="resource.descriptio"
      :link="resource.link"
      :id="resource.id"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from "./LearningResource.vue";
export default {
  components: { LearningResource },
  inject: ["resources"],
  data() {},
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
