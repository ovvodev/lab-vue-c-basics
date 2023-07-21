<script setup>
import { ref } from 'vue';

const articles = ref([
    {
        title: "The old town",
        description: "This is the oldest town in this region",
        content: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet."
    },
    {
        title: "The new town",
        description: "This is the newest town in this region",
        content: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet."
    },
    {
        title: "The region",
        description: "This is the region",
        content: "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet."
    },

]);

</script>

<template>
  <ul>
    <li v-for="article in articles" :key="article.title">
        <h3>{{ article.title }}</h3>
        <p>{{ article.description }}</p>
        <p>{{ article.content }}</p>
    </li>
  </ul>
  <br>
  
</template>

<style scoped>

</style>
