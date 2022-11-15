<template>
  <h1>Listado de Posts:</h1>
  <PostContainer />
  <br>
  <CounterOption />
</template>

<script lang="ts" setup>
  import PostContainer from './components/PostContainer.vue';
  import CounterOption from './components/CounterOption.vue';
</script>

<style>
  h1 {
    color: green;
  }
</style>
