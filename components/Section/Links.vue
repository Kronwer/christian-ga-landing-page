<script setup>
import { _white } from '#tailwind-config/theme/accentColor';
import { ref } from 'vue'

const email = 'christiangarcia11598@gmail.com'
const phone = '+34692618440'
const copied = ref(false)
const toast = useToast()

const copyToClipboard = (value) => {
    navigator.clipboard.writeText(value)
    .then(() => {
      copied.value = true
      setTimeout(() => copied.value = false, 2000)
      toast.add({
        title: 'Copied to clipboard!',
        icon: 'uil:clipboard-notes',
        timeout: 2000,
      })
    })
    .catch(err => {
      console.error('Failed to copy text: ', err)
    })
}
</script>

<template>
    <div class="flex flex-col gap-2">
        <div>
            <p class="font-semibold text-lg md:text-xl text-center">Contact Me</p>
        </div>
        <div class="flex justify-center gap-8">
            <UTooltip text="Open in new tab">
                <a href="https://www.linkedin.com/in/christianga/" target="_blank" rel="noopener noreferrer">
                    <Icon name="uil:linkedin" size="3em" style="color: white" />
                </a>
            </UTooltip>
            <UTooltip text="Click to copy">
                <Icon name="uil:envelope" size="3em" style="color: white"
                    @click=copyToClipboard(email) />
            </UTooltip>
            <UTooltip text="Click to copy">
                <Icon name="uil:phone" size="3em" style="color: white"
                    @click=copyToClipboard(phone) />
            </UTooltip>
            <UTooltip text="Open in new tab">
                <a href="https://github.com/Kronwer" target="_blank" rel="noopener noreferrer">
                    <Icon name="uil:github" size="3em" style="color: white" />
                </a>
            </UTooltip>
        </div>
    </div>
</template>