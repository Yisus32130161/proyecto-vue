<template>
    <Header :mensaje="texto"></Header>
    <div class="container">
        <Sidebar></Sidebar>
        <di class="content">
            <input type="texto" v-model="texto">
            {{ texto }}
            <RouterView></RouterView>
        </di>
    </div>
</template>

<script setup>
import Sidebar from '../components/Sidebar.vue';
import Header from '../components/Header.vue';
import { ref } from 'vue';
const texto = ref('');
</script>

<style>
.container {
    display: flex;
}
.content {
    flex: 1;
    padding: 20px;
}
</style>