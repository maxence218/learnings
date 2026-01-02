<script setup>
  defineProps({
    texte: { type: String, default: "clickme" }
  })
</script>


<template>
  <button class="btn"> {{ texte }} </button>
</template>


<style scoped>

</style>
