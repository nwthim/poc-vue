<template>
  <q-layout view="lHh Lpr lFf">
    <header class="container py-8 mx-auto prose">
      <h1>{{ title }}</h1>
    </header>
    <q-page-container>
      <router-view />
    </q-page-container>
    <footer class="container py-6 mx-auto text-center text-gray-700">
      <p>
        Cute footer &copy; .
      </p>
    </footer>
  </q-layout>
</template>

<script setup lang="ts">
const props = defineProps<{
  title?: string
}>()
</script>

