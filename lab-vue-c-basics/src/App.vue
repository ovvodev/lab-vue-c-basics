<script setup>
import { ref } from 'vue';
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';


const newCss = ref("app-new");

function toggleTheme() {
  newCss.value = newCss.value === "app-new" ? "" : "app-new";
}
</script>

<template>
  <section :class="newCss">
    <NavBar></NavBar>
    <Footer></Footer>
    <button @click="toggleTheme">Change Theme</button>
  </section>
  
</template>

<style>
.app-new {
    background-color: black;
    color: white;
}
</style>
