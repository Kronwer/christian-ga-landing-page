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
                <p class="font-bold">{{ props.companyName }}</p>
                <p class="text-sm">{{ props.title }}</p>
                <p class="text-xs mb-2">{{ props.period }}</p>
                <p class="text-xs text-slate-400">Keywords: {{ props.technologies }}</p>
            </div>
        </div>
</template>