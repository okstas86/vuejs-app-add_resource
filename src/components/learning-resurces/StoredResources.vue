<template>
  <ul>
    <learning-resuorce
      v-for="res in resources"
      :key="res.id"
      :id="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    ></learning-resuorce>
  </ul>
</template>

<script>
import LearningResuorce from './LearningResuorce.vue';
export default {
  inject: ['resources'],
  components: { LearningResuorce },
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
