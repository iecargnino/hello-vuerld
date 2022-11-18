<template>
  <h1>Listado de Posts:</h1>
  <PostContainer />
  <br>
  <CounterOption />
  <br>
  <CounterComposition />
  <ExampleSelectiveVue />
  <br>
  <ExampleFor />
  <br>
  <ClassBind />
  <br>
  <EventsBind />
  <br>
  <ModelForm />
</template>

<script lang="ts" setup>
  import PostContainer from './components/PostContainer.vue';
  import CounterOption from './components/CounterOption.vue';
  import CounterComposition from './components/CounterComposition.vue';
  import ExampleSelectiveVue from './components/ExampleSelective.vue';
  import ExampleFor from './components/ExampleFor.vue';
  import ClassBind from './components/ClassBind.vue';
  import EventsBind from './components/EventsBind.vue';
  import ModelForm from './components/ModelForm.vue';
</script>

<style>
  h1 {
    color: green;
  }
</style>
