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
            <UDivider :avatar="{src: imageUrl, size: 'sm'}" orientation="vertical" size="md" />
            <div>
                <p class="font-bold lg:text-lg xl:text-xl">{{ props.collegeName }}</p>
                <p class="text-sm lg:text-sm xl:text-base">{{ props.title }}</p>
                <p class="text-xs text-slate-200 lg:text-sm xl:text-base">{{ props.period }}</p>
            </div>
        </div>
</template>