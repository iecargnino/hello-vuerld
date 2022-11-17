<template>
    <ul>
        <!--<li v-for="pais in countries" v-bind:key="pais">{{ pais }}</li> -->
        <li v-for="pais in countries" v-bind:key="pais.code">{{ pais.name }}</li>
    </ul>
</template>
  
<script lang="ts" setup>
    import { Ref, ref } from 'vue';
    /*let countries:Ref<Array<string>> = ref([
        'Argentina', 'España', 'Uruguay', 'Brasil', 'Italia', 'Africa'
    ])*/
    interface ICountry {
        code: string,
        name: string
    }
    
    let countries:Ref<Array<ICountry>> = ref([
        {
            code: 'Ar',
            name: 'Argentina'
        },
        {
            code: 'Es',
            name: 'España'
        },
        {
            code: 'Ur',
            name: 'Uruguay'
        },
        {
            code: 'Br',
            name: 'Brasil'
        },
        {
            code: 'It',
            name: 'Italia'
        },
        {
            code: 'Af',
            name: 'Africa'
        }
    ])
</script>
  
<style scoped>
</style>