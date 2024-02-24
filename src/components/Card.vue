<script setup>
defineProps({
    imageUrl: String,
    title: String,
    price: Number,
    isFavorite: Boolean,
    isAdded: Boolean,
    onClickAdd: Function,
    onClickFavorite: Function
})

</script>
<template>
    <div class="relative 
        bg-white border 
        border-slate-100 
        rounded-3xl p-8 
        cursor-pointer 
        transition hover:-translate-y-2 hover:shadow-xl">
          <img :src="isFavorite ? '/like-2.svg': 'like-1.svg'" 
                class="absolute top-0 left-0" 
                @click="onClickFavorite"/>
          
                <img :src="imageUrl" class="w-full"/>
          <p class="mt-2">{{ title }}</p>
          <div class="flex justify-between mt-5">
            <div class="flex flex-col">
              <span class="text-slate-400">Price</span>
              <b>{{ price }}</b>
            </div>
            <img :src="isAdded ? '/checked.svg': '/plus.svg'" @click="onClickAdd">
          </div>
        </div>
</template>