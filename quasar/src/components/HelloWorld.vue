<template>
  <div>
    <h2>{{ msg }}</h2>
    <q-btn class="px-3 py-2 border border-gray-300 rounded-md shadow" @click="increment">
      count is: {{ count }}
    </q-btn>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0);
defineProps<{
  msg: string
  optionalProp?: number
}>()

function increment() {
  count.value += 1;
}
</script>
