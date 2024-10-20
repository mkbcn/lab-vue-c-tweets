<template>
        <span class="timestamp">{{ timestamp }} </span>
</template>

<script setup>
    import {defineProps} from 'vue'
 
    defineProps({
        timestamp: String
        })
</script>

<style scoped>

</style>