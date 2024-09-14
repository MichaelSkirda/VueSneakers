<script setup>

import MultiStateButton from './MultiStateButton.vue'

defineProps({
    title: String,
    price: Number,
    imageSrc: String,
    imageAlter: String,
    isFavourite: Boolean,
    isAdded: Boolean
})

const addToCartStates = [
    {
        src: '/plus.svg',
        alt: 'Add to cart'
    },
    {
        src: '/checked.svg',
        alt: 'Remove from cart'
    }
]

const addToFavouriteStates = [
    {
        src: '/like-1.svg',
        alt: 'Add to fovourite'
    },

    {
        src: '/like-2.svg',
        alt: 'Remove from favourite'
    }
]

</script>

<template>
    <div class="relative border border-slate-200 rounded-3xl p-8 cursor-pointer transition duration-150 hover:-translate-y-2 hover:shadow-xl">

        <MultiStateButton
                class="absolute top-8 left-8"
                :states="addToFavouriteStates" 
            />

        <img :src="imageSrc" :alt="imageAlter ?? 'Sneakers'">

        <p>{{ title }}</p>

        <div class="flex justify-between mt-2">
            
            <div class="flex flex-col">
                <span class="text-slate-400 leading-tight">Цена:</span>
                <b class="leading-tight">{{ price }} руб.</b>
            </div>

            <MultiStateButton
                :states="addToCartStates" 
            />

        </div>
            
    </div>
</template>