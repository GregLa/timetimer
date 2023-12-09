<script setup>
import Button from '@/components/designsystem/Button.vue'
import CircleButton from '@/components/designsystem/CircleButton.vue'
</script>
<template>
    <div class="wrapper">
        <Button class="addTime" text="+1'"></Button>
        <CircleButton></CircleButton>
        <Button class="addTime" text="+5'"></Button>
    </div>
</template>
<style scoped>
.wrapper {
    display: flex;
    align-items: center;
    gap: var(--size-40-px, 2.5rem);
}
</style>