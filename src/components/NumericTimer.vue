<script setup>
import NumericDisplay from '@/components/NumericDisplay.vue';
import TimerController from '@/components/TimerController.vue';
import Toaster from '@/components/Toaster.vue';
import TimeSelector from '@/components/TimeSelector.vue';
import { ref } from 'vue';

const timerActive = ref(false)

const handleStart = (time) => {
    console.log(time)
    timerActive.value = true;
}

</script>
<template>
    <div class="numeric-timer">
        <TimeSelector 
            @start-timer="handleStart"
            :class="{ hide: timerActive }"
            ></TimeSelector>
        <Toaster class="toaster" />
        <NumericDisplay :class="{ hide: !timerActive }" />
        <TimerController :class="{ hide: !timerActive }" />
    </div>
</template>
<style scoped>
.numeric-timer {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    height: 100%;
}

.toaster {
    height: 100px;
}

.hide {
    display: none;
}
</style>