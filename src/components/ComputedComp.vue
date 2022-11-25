<template>
    <div>
        <label>Subtotal</label>
        <input type="number" v-model="subtotal">
        <h3>Impuesto a pagar: {{ totalVat }} ({{ vat }}%)</h3>
    </div>
</template>


<script lang="ts" setup>
    import { Ref, ref, computed } from 'vue';

    let vat = 0.21

    const subtotal:Ref<number> = ref(0)

    const totalVat = computed( () => (vat*subtotal.value))
</script>

<style></style>
