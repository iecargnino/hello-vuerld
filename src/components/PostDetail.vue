<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
        <button @click="handleCLick">Saludar</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'PostDetail',
        props: {
            title: {
                type: String,
                required: true
            },
            content: {
                type: String,
                required: false,
                default: 'Este post no tiene Texto'
            }
        },
        emits: ['sayHi'],
        setup(props, {emit}) {
            const handleCLick = () => {
                emit('sayHi', 'Hola Wachin!')
            }
            return { props, handleCLick }
        }
    })
</script>

<style scoped>
    .post {
        width: 200px;
        height: 100px;
        background-color: antiquewhite;
        border-radius: 10px;
        margin: 10px;
        padding: 10px
    }
</style>