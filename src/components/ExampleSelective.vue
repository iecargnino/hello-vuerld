<template>
    <h1 v-if="edad < 10">Eres menor de edad</h1>
    <h1 v-else>Eres mayor de edad</h1>
  </template>
  
  <script lang="ts" setup>
    let edad = 8
  </script>
  
  <style scoped>
    h1 {
      color: green;
    }
  </style>