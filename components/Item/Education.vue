<script setup>
const props = defineProps({
    imageUrl: {
        type: String,
        required: true
    },
    collegeName: {
        type: String,
        required: true
    },
    title: {
        type: String,
    },
    period: {
        type: String
    }
})
</script>

<template>
        <div class="flex gap-3">
            <UDivider :avatar="{src: imageUrl}" orientation="vertical" size="md" />
            <div>
                <p class="font-bold">{{ props.collegeName }}</p>
                <p class="text-sm">{{ props.title }}</p>
                <p class="text-xs text-slate-200">{{ props.period }}</p>
            </div>
        </div>
</template>