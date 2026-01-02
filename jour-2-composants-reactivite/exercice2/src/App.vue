<script setup>
  import { ref } from 'vue'
  import Compteur from './component/Compteur.vue'
  const liste = ref(["lait", "beurre", "farine"])
</script>

<template>
  <Compteur/>
  <li v-for="(message, index) in liste" :key="index">{{ index + 1 }} - {{ message }}</li>
</template>

<style scoped>

</style>
