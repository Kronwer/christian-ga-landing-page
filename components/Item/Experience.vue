<script setup>
const props = defineProps({
    imageUrl: {
        type: String,
        required: true
    },
    companyName: {
        type: String,
        required: true
    },
    title: {
        type: String
    },
    period: {
        type: String
    },
    technologies: {
        type: String
    }
})
</script>

<template>
        <div class="flex gap-3">
            <UDivider :avatar="{src: imageUrl}" orientation="vertical" size="md" />
            <div>
                <p class="font-bold text-sm">{{ props.companyName }}</p>
                <p class="text-xs">{{ props.title }}</p>
                <p class="text-xs">{{ props.period }}</p>
                <p class="text-xs">Keywords: {{ props.technologies }}</p>
            </div>
        </div>
</template>