<template>
    <p v-bind:style="{ backgroundColor : '#ccc', color : c }">Mensaje enviado correctamente</p>
    <button v-on:click="changeColor()">CAMBIAR</button>
</template>
  
<script lang="ts" setup>
    import { ref } from 'vue'
    let c = ref('#fff')
    const changeColor = () => { c.value = '#ff0000'}
</script>
  
<style>
</style>