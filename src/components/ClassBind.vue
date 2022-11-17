<template>
    <p v-bind:class="{ danger: hasError }">Mensaje enviado correctamente</p>
</template>
  
<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'ClassBind',
        setup() {
            let hasError = false;
            return { hasError }
        }
    })
</script>
  
<style scoped>
    .danger {
      color: red;
    }
</style>