<script setup>
import Card from './Card.vue'

const addProduct = () => alert('add!')
const addFavorite = () => alert('Favorite')
</script>
<template>
    <div class="grid grid-cols-1 gap-5 mt-10 md:grid-cols-2 lg:grid-cols-4">
        <Card 
            image-url="/sneakers/sneakers-1.jpg" 
            title="Nike Blazer Mid 77 - Pine green" 
            price="500,00"
            :onClickAdd="addProduct"
            :onClickFavorite="addFavorite"
        />
        
        <Card 
            image-url="/sneakers/sneakers-1.jpg" 
            title="Nike Blazer Mid 77 - Pine green" 
            price="500,00"
            :onClickAdd="addProduct"
            :onClickFavorite="addFavorite"
        />
    </div>
</template>