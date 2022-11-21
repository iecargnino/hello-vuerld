<template>
    <h3>Hola gente Linda!</h3>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'CycleOption',
        created() {
            console.log('Creado!')
        },
        mounted() {
            console.log('Montado!')  
        },
        updated() {
            console.log('Actualizado!')
        },
        unmounted() {
            console.log('Destruido!')
        },
    })

</script>