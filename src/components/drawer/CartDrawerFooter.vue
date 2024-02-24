<template>
    <div class="flex flex-col gap-3 my-7">
            <div class="flex gap-2 ">
                <span>Total</span>
                <div class="flex-1 border-b border-dashed"></div>
                <b>$ 500,00</b>
            </div>
            
            <div class="flex gap-2 ">
                <span>Desconto 5%</span>
                <div class="flex-1 border-b border-dashed"></div>
                <b>$ 475,00</b>
            </div>
        </div>
        <button 
             disabled
             class="bg-lime-500
             disabled:bg-slate-400
             hover:bg-lime-600
             active:bg-lime-700 
             cursor-pointer
             w-full rounded-xl py-3 text-white font-bold mt-2">Concluir Pedido</button>
</template>