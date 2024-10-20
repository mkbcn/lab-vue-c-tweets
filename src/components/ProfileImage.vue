<template>
    <img 
    :src="image" 
    class="profile" 
    alt="profile"/>
</template>


<script setup>
    import {defineProps} from 'vue'

    defineProps({
        image: String
        })
</script>

<style scoped>

</style>