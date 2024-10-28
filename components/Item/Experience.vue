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
                <p class="font-bold lg:text-lg xl:text-xl">{{ props.companyName }}</p>
                <p class="text-sm lg:text-base xl:text-lg">{{ props.title }}</p>
                <p class="text-xs mb-2 lg:text-sm xl:text-base">{{ props.period }}</p>
                <p class="text-xs text-slate-400 lg:text-sm">Keywords: {{ props.technologies }}</p>
            </div>
        </div>
</template>