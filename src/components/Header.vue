<template>
    <header class="flex justify-between border-b border-slate-200 p-8">
      <div class="flex items-center gap-4">
        <img src="/logo.png" class="w-10"/>
        <div>
          <h2 class="text-xl font-bold uppercase">Sneack Store</h2>
          <p class="text-slate-400 text-xs font-thin">Os melhor encontra-se aqui</p>
        </div>
      </div>

      <ul class="flex items-center gap-10 ">
        <li class="flex items-center cursor-pointer gap-2 text-gray-500 hover:text-black">
          <img src="/cart.svg" alt="">
          <b>1205 py6.</b>
        </li>
        <li class="flex items-center cursor-pointer gap-2 text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="">
          <span>favorite</span>
        </li>
        <li class="flex items-center cursor-pointer gap-2 text-gray-500 hover:text-black">
          <img src="/profile.svg" alt="">
          <span>profile</span>
        </li>
      </ul>
    </header>
</template>