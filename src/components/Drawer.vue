<script setup>
import DrawerHeader from './drawer/DrawerHeader.vue'
import CartDrawerList from './drawer/CartDrawerList.vue'
import CartDrawerFooter from './drawer/CartDrawerFooter.vue'
</script>
<template>
    <div class="fixed top-0 left-0 h-full w-full bg-black bg-opacity-70 z-10"></div>
    <div class="flex flex-col bg-white w-full sm:w-96 h-full fixed right-0 top-0 z-20 p-5 ">
        <DrawerHeader/>
        <CartDrawerList/>
        <CartDrawerFooter/>
    </div>
</template>