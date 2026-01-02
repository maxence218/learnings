<script setup>
  import { ref } from 'vue'
  const count = ref(0)
  import Bouton from './Bouton.vue'
  function increment() {
    count.value++
  }
  function decrement() {
    count.value--
  }
  function reset() {
    count.value = 0
  }
</script>

<template>
  <div>
    <p v-if="count > 0" style="color: green; font-weight: bold"> {{ count }}</p>
    <p v-else style="color: red; font-weight: bold">{{ count }}</p>
  </div>
  <Bouton texte="incremente" @click="increment"/>
  <Bouton texte="decremente" @click="decrement"/>
  <Bouton texte="reset" @click="reset"/>
</template>

<style scoped>
</style>
