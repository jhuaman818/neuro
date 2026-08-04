<template>
    <button
        :class="['btn', `btn-${variant}`, { 'btn-disabled': disabled }]"
        :disabled="disabled"
        @click="$emit('click')">
        <slot />
    </button>
</template>


<script setup>
defineProps({
    variant: {
        type: String,
        default: 'primary'
    },
    disabled: {
        type: Boolean,
        default: false
    }
})
</script>