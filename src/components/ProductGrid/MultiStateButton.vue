<script setup>

import { computed, ref } from 'vue'

const props = defineProps({
    startIndex: {
        type: Number,
        default: 0
    },
    states: Array,
    clickCallback: Function
})

const states = props.states;

let index = ref(props.startIndex)
const maxIndex = states.length

const state = computed(() => {
    return states[index.value];
})

const incrementState = () => {
    index.value = (index.value + 1) % maxIndex
    if(props.clickCallback)
        props.clickCallback()
}

</script>

<template>
    <img @click="incrementState" :src="state.src" :alt="state.alt">
</template>