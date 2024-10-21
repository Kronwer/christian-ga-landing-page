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
    }
})
</script>

<template>
    
        <div class="flex gap-4 items-start">
            <UAvatar :src=imageUrl size="lg" />
            <div>
                <p class="font-semibold text-lg">{{ props.collegeName }}</p>
                <p class="text-sm">{{ props.title }}</p>
            </div>
        </div>
    
</template>