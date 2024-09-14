<script setup>

import ProductItem from './ProductItem.vue'

</script>

<template>

    <div class="p-12">
        <h2 class="text-3xl font-bold">Все кроссовки</h2>

        <div class="grid grid-cols-4 gap-8 mt-10">
            <ProductItem title="Мужские Кроссовки Nike Blazer Mid Suede" imageSrc="/sneakers/sneakers-1.jpg" imageAlter="Green nike sneakers" :price="12999"/>
            <ProductItem title="Мужские Кроссовки Nike Blazer Mid Suede" imageSrc="/sneakers/sneakers-1.jpg" imageAlter="Green nike sneakers" :price="12999"/>
            <ProductItem title="Мужские Кроссовки Nike Blazer Mid Suede" imageSrc="/sneakers/sneakers-1.jpg" imageAlter="Green nike sneakers" :price="12999"/>
            <ProductItem title="Мужские Кроссовки Nike Blazer Mid Suede" imageSrc="/sneakers/sneakers-1.jpg" imageAlter="Green nike sneakers" :price="12999"/>
            <ProductItem title="Мужские Кроссовки Nike Blazer Mid Suede" imageSrc="/sneakers/sneakers-1.jpg" imageAlter="Green nike sneakers" :price="12999"/>
        </div>
    </div>
    
</template>