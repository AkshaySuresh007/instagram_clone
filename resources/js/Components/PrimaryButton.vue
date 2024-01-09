<script setup>
defineProps({
    type: {
        type: String,
        default: "submit",
    },
    color: {
        type: String,
        default: "bg-[#0095F6] hover:bg-[#2150fa]"
    }
});
</script>

<template>
    <button
        :type="type"
        :class="color"
        class="w-full rounded-lg p-1.5 text-white text-lg font-extrabold"
    >
        <slot />
    </button>
</template>
