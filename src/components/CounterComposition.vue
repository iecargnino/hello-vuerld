<template>
    <h3>{{ counter }}</h3>
    <div class="counter-div">
        <button @click="addCounter">+</button>
        <button @click="restCounter">-</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent, ref } from 'vue';
    export default defineComponent({
        name: 'CounterOption',
        setup() {
            let counter = ref(0);
            const addCounter = () => {
                counter.value++;
                console.log(counter)
            };
            const restCounter = () => {
                counter.value--;
            }
            return { counter, addCounter, restCounter }
        }
    })
</script>

<style scoped>
    .counter-div, h3 {
        text-align: center;
    }
</style>
