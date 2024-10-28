<template>
  <h1>Hola mundo</h1>
 <p> {{ contador }}</p>
  <button @click="incremental">incremental</button>
  <button @click="decrememtal">decrememtal</button>
</template>

<script setup>
import { ref } from 'vue';
const contador = ref(0);
const incremental = () => {
  contador.value++;
}
const decrememtal = () => {
  contador.value--;
}
</script>

<style scoped>
p{
  color: red;
}
</style>
