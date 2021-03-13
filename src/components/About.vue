<template>
    <h1 class="text-2xl font-bold">About {{ name }}</h1>
</template>

<script setup>
import { computed } from 'vue'
import { useStore } from 'vuex'
const store = useStore()

const name = computed(() => {
    return store.state.user.name
})
</script>
