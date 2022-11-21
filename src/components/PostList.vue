<template>
    <div class="container">
        <PostDetail v-for="item in info" :key="item.title" :title="item.title" :content="item.content" @sayHi="showAlert"/>
    </div>
</template>

<script lang="ts" setup>
    import PostDetail from './PostDetail.vue';
    
    interface Post {
        title: string,
        content: string
    }

    let info:Array<Post> = [
        {
            title: 'Este es el post 1',
            content: 'Texto ejemplo 1'
        },
        {
            title: 'Este es el post 2',
            content: 'Texto ejemplo 2'
        },
        {
            title: 'Este es el post 3',
            content: 'Texto ejemplo 3'
        },
        {
            title: 'Este es el post 4',
            content: 'Texto ejemplo 4'
        },
        {
            title: 'Este es el post 5',
            content: 'Texto ejemplo 5'
        }]

        function showAlert(msg:string) {
            alert(msg)
        }

</script>

<style scoped>
    .container {
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        justify-content: space-around;
    }
</style>