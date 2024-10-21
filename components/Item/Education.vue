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
    
        <div class="flex gap-4 md:items-center">
            <UAvatar :src=imageUrl size="lg" />
            <div>
                <p class="font-semibold text-lg">{{ props.collegeName }}</p>
                <p class="text-sm">{{ props.title }}</p>
                <p class="text-xs">{{ props.period }}</p>
            </div>
        </div>
    
</template>