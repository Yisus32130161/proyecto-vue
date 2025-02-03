<template>
<div class="container">
    <Sidebar></Sidebar>
    <di class="content">
        <RouterView></RouterView>
    </di>
</div>
</template>

<script setup>
import Sidebar from '../components/Sidebar.vue';
</script>

<style>
.conatiner {
    display: flex;
}
.content {
    flex: 1;
    padding: 20px;
}
</style>