<script setup>
defineProps({
    icon: {
        type: String,
        default: "play_pause"
    }
})
</script>
<template>
    <button>
        <span class="material-symbols-outlined">
            {{ icon }}
        </span>
    </button>
</template>
<style scoped>
button {
    cursor: pointer;
    display: flex;
    width: 6.5rem;
    height: 6.5rem;
    padding: 2rem 2.25rem;
    justify-content: center;
    align-items: center;
    border-radius: 12.5rem;
    border-top: 4px solid rgba(199, 210, 221, 0.50);
    border-right: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-bottom: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-left: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    background: var(--colors-button-bg, #FFF);

    span {
        display: flex;
        align-items: flex-start;
    }
}
</style>