<template>
    <p class="message">{{message}}</p>
</template>
 
<script setup>
    import {defineProps} from 'vue'

    defineProps({
        message: String
        })
</script>
   
<style scoped>


</style>