<script setup lang="ts">
import { ref } from 'vue'

const likes = ref(3)

const handleClick = () => {
    likes.value++
}
</script>

<template>
    <div class="likes">
        <p>{{ likes }} people like this review.</p>
        <button @click="handleClick">Like</button>
    </div>
</template>
