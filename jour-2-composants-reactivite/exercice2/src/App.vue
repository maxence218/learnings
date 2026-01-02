<script setup>
  import { ref } from 'vue'
  import Compteur from './component/Compteur.vue'
  const liste = ref(["lait", "beurre", "farine"])
</script>

<template>
<Compteur/>

  <li v-for="(message, index) in liste">{{ index }} - {{ message }}</li>

</template>

<style scoped></style>
