<template>
    <form>
        <br>
        <input type="text" v-model="inputText" />
        <br>
        <input type="checkbox" v-model="agree" /> Acepto los términos y condiciones
        <br>
        <select v-model="selectOption">
            <option value="Arg">Argentina</option>
            <option value="Br">Brasil</option>
            <option value="Pe">Peru</option>
        </select>
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import { ref } from 'vue'
    let inputText = ref('')
    let agree = ref(true)
    let selectOption = ref('Pe')
</script>

<style>
</style>