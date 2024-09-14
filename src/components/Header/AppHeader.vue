<script setup>

import LogoItem from './LogoItem.vue'

</script>

<template>
    <header class="flex justify-between border-b border-slate-200 px-10 py-8">
        
            <LogoItem/>

            <ul class="flex items-center gap-10">
                <li class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black">
                    <img src="cart.svg" alt="cart">
                    <b>1205 руб.</b>
                </li>
                <li class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black">
                    <img src="heart.svg" alt="cart">
                    <span>Закладки</span>
                </li>
                <li class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black">
                    <img src="profile.svg" alt="cart">
                    <span>Профиль</span>
                </li>
            </ul>

        </header>
</template>