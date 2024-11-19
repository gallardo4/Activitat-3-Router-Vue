<script setup>
import productList from '@/assets/products.json'
import { RouterLink } from 'vue-router'
</script>

<template>
    <ul>
        <li v-for="product in productList" :key="product.id">
            <RouterLink :to="'/productDetail/' + product.id + '/' + product.name + '/' + product.description">{{ product.name }}</RouterLink>
        </li>
    </ul>
</template>

<style scoped>

li {
    padding: 0.5rem;
}

</style>