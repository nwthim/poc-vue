<template>
  <div class="border mb-4">
    <img :src="img" />
    <div>{{ text }}</div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  img: string
  text?: string
}>()
</script>
