<script setup>
import Button from '@/components/designsystem/Button.vue';
defineEmits(['startTimer'])
</script>
<template>
    <div class="wrapper">
        <Button class="addTime" text="5'" size="big" @click="$emit('startTimer', 5)"></Button>
        <Button class="addTime" text="10'" size="big" @click="$emit('startTimer', 10)"></Button>
        <Button class="addTime" text="15'" size="big" @click="$emit('startTimer', 15)"></Button>
        <Button class="addTime" text="30'" size="big" @click="$emit('startTimer', 30)"></Button>
        <Button class="addTime" text="60'" size="big" @click="$emit('startTimer', 60)"></Button>
    </div>
</template>
<style scoped>
.wrapper {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: var(--size-40-px, 2.5rem);
}
</style>