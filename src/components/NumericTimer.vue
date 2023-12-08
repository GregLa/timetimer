<script setup>
</script>
<template>
    <div class="wrapper">
        <div class="timer">
            <div class="digit">0</div>
            <div class="digit">4</div>
            <div class="separator">:</div>
            <div class="digit">5</div>
            <div class="digit">9</div>
        </div>
    </div>
</template>
<style scoped>
.wrapper {
    display: flex;
    flex-direction: column;
}

.timer {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: var(--size-24-px, 1.5rem);
    flex: 1 0 0;
    align-self: stretch;
}

.digit {
    display: flex;
    width: 7.3125rem;
    padding: var(--size-24-px, 1.5rem);
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 0.5rem;
    border-radius: var(--size-16-px, 1rem);
    background: var(--colors-analog-timer, #F9FCFF);
    box-shadow: 0px 2px 6px 0px rgba(71, 74, 77, 0.25) inset;
    color: var(--colors-text, #26282B);
    font-family: SF Pro Text;
    font-size: 6.25rem;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.separator {
    display: flex;
    width: 2.4375rem;
    flex-direction: column;
    justify-content: center;
    align-self: stretch;
    color: var(--colors-text, #26282B);
    text-align: center;
    font-family: SF Pro Text;
    font-size: 6.25rem;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}
</style>