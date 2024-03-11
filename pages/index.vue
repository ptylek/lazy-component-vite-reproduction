<template>
    <div class="index">
        <LazyMarker v-if="toggle" />
        <button @click="toggle = !toggle">toggle</button>
        {{ getTestString('homepage') }}
    </div>
</template>

<script setup>
import { getTestString } from '@/my-utils/getTestString'
const toggle = ref(false)
</script>

<style>
.index {
    height: 100vh;
    width: 100%;
    background: red;
}
</style>