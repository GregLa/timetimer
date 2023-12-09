<script setup>
defineProps({
    text: String,
    size: {
        type: String,
        default: "small",
        validator(value) {
            return ['xsmall', 'small', 'big'].includes(value)
        }
    }
})
</script>
<template>
    <button :class="size">
        <span>
            {{ text }}
        </span>
    </button>
</template>
<style scoped>
button {
    cursor: pointer;
    font-family: 'Roboto', sans-serif;
}
.big {
    display: inline-flex;
    padding: var(--size-24-px, 1.5rem) var(--size-40-px, 2.5rem);
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: var(--size-8-px, 0.5rem);
    border-radius: var(--size-56-px, 3.5rem);
    border: 4px solid rgba(199, 210, 221, 0.50);
    background: var(--colors-button-bg, #FFF);

    span {
        color: var(--colors-text, #26282B);
        font-size: 2.5rem;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
}

.small {
    display: inline-flex;
    padding: var(--size-16-px, 1rem) var(--size-24-px, 1.5rem);
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: var(--size-8-px, 0.5rem);
    border-radius: var(--size-56-px, 3.5rem);
    border-top: 4px solid rgba(199, 210, 221, 0.50);
    border-right: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-bottom: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-left: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    background: var(--colors-button-bg, #FFF);

    span {
        color: var(--colors-text, #26282B);
        font-size: 1.875rem;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
}

.xsmall {
    display: inline-flex;
    padding: var(--size-8-px, 0.5rem) var(--size-16-px, 1rem);
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: var(--size-8-px, 0.5rem);
    border-radius: var(--size-56-px, 3.5rem);
    border-top: 4px solid rgba(199, 210, 221, 0.50);
    border-right: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-bottom: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    border-left: var(--size-4-px, 4px) solid rgba(199, 210, 221, 0.50);
    background: var(--colors-button-bg, #FFF);

    span {
        color: var(--colors-text, #26282B);
        font-size: 1.25rem;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
}</style>