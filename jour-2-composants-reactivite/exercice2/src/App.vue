<script setup>
  import { ref } from 'vue'
  import Compteur from './component/Compteur.vue'
  const liste = ref(["lait", "beurre", "farine"])
</script>

<template>
<Compteur/>
<ul>
  <li v-for="message in liste"> {{ message }}</li>
</ul>
</template>

<style scoped></style>
