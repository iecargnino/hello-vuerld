<template>
    <h3>{{ counter }}</h3>
    <div class="counter-div">
        <button @click="addCounter">+</button>
        <button @click="restCounter">-</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'CounterOption',
        data() {
            let counter = 0;
            return { counter }
        },
        methods: {
            addCounter() {
                this.counter++
            },
            restCounter() {
                this.counter--
            }
        }
    })
</script>

<style scoped>
    .counter-div, h3 {
        text-align: center;
    }
</style>
