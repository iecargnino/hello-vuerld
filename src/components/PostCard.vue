<template>
    <div class="post-card">
        <h3>TITULO</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea consequuntur quam officiis iusto nisi possimus reiciendis, amet aperiam deserunt, ex vel. Tenetur suscipit alias mollitia, iure nostrum autem ab molestias!</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
    import PostButton from './PostButton.vue';
</script>

<style scoped>
    .post-card {
        border-radius: 15px;
        padding: 10px;
        margin: 5px;
        border: 1ps solid #ccc;
    }
</style>