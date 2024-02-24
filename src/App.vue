<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
// import Drawer from './components/Drawer.vue';
</script>

<template>
   <!-- <Drawer/>  -->
   <div class="bg-white w-full sm:w-4/5 m-auto rounded-xl shadow-xl sm:mt-14">
      <Header/>
      <div class="p-10">
        <div class="flex flex-col gap-5 md:flex-row  justify-between items-center">
          <h2 class="w-full text-3xl font-bold text-center md:text-justify lg:w-70">Conheça nossas ofertas</h2>
          <div class="relative w-full lg:w-60">
            <img src="./assets/icons/search.svg" class="absolute right-3 top-2.5" >
            <input type="text" placeholder="Search ..." 
              class="sm:w-full  border rounded-md py-1.5 pl-10 pr-4 outline-none focus:border-gray-400">
          </div>
        </div>
        <CardList/>
      </div>  
   </div>
</template>

