<script setup>
import Card from './Card.vue'

defineProps({
    items: Array
})

const addProduct = () => alert('add!')
const addFavorite = () => alert('Favorite')
</script>
<template>
    <div class="grid grid-cols-1 gap-5 mt-10 md:grid-cols-2 lg:grid-cols-4">
        <Card v-for="item in items" :key="item.id"
            :image-url="item.imageUrl" 
            :title="item.title" 
            :price="item.price"
            :onClickAdd="addProduct"
            :onClickFavorite="addFavorite"
        />
    </div>
</template>