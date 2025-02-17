<script setup>
import {defineProps} from 'vue';

defineProps({
    bgClass: {
        type: String,
        default: 'bg-gray-100'
    }
})
</script>

<template>
    <div :class="`${bgClass} p-6 rounded-lg shadow-md`">
        <slot></slot>
    </div>
</template>