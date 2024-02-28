<script setup>
import { onMounted, ref } from 'vue'
import axios from 'axios'

import Header from './components/Header.vue'
import CardList from './components/CardList.vue'

const items = ref([])

onMounted(async () => {
  const {data} = await axios.get('https://c78fcbd28c0149aa.mokky.dev/items')
  items.value = data
})

</script>

<template>
   <!-- <Drawer/>  -->
   <div class="bg-white w-full m-auto rounded-xl shadow-xl sm:mt-14">
      <Header/>
      <div class="p-10">
        <div class="flex flex-col gap-5 md:flex-row  justify-between items-center">
          <h2 class="w-full text-2xl font-bold text-center md:text-justify lg:w-70">Conheça nossas ofertas</h2>
          <div class="flex flex-col gap-4">
            <select class="border py-2 px-3 rounded-md">
              <option value="">1</option>
              <option value="">2</option>
              <option value="">3</option>
            </select>
            <div class="relative">
              <img src="./assets/icons/search.svg" class="absolute right-3 top-2.5" >
              <input type="text" placeholder="Search ..." 
                class="w-full border rounded-md py-2 px-3 outline-none focus:border-gray-400">
            </div>
          </div>
        </div>
        <CardList :items="items"/>
      </div>  
   </div>
</template>

