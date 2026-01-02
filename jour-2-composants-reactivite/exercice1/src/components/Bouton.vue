<script setup>
defineProps({
  texte: {type: String, default: "click-me"},
  couleur: {type: String, default: "#2874a6"}
})
</script>


<template>
  <button class="btn" :style="{ backgroundColor: couleur }">{{ texte }}</button>
</template>


<style scoped>
  .btn {
    padding: 10px 20px;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    margin: 5px;
  }
</style>
