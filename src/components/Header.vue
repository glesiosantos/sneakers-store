<template>
    <header class="flex justify-center border-b border-slate-200 py-8 px-5">
      <div class="flex items-center w-full gap-3">
        <img src="/logo.png" class="w-10"/>
        <div>
          <h2 class="text-xl font-bold uppercase">Sneack Store</h2>
          <p class="text-slate-400 text-xs font-thin">Os melhor encontra-se aqui</p>
        </div>
      </div>

      <ul class="flex items-center">
        <li class="flex cursor-pointer text-gray-500 hover:text-black">
          <img src="/cart.svg" alt="">
          <b class="invisible md:visible">1205 py6.</b>
        </li>
        <li class="flex cursor-pointer text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="">
          <span class="invisible md:visible">favorite</span>
        </li>
        <li class="flex cursor-pointer text-gray-500 hover:text-black">
          <img src="/profile.svg" alt="">
          <span class="invisible md:visible">profile</span>
        </li>
      </ul>
    </header>
</template>