<template>
  <q-page class="row items-center justify-evenly">
    <div class="container mx-auto prose prose-purple">
      <HelloWorld opt msg="Quasar + Vue 3 + SSR" />

      <hr />

      <h2>Render 100 boxes</h2>
      <Box v-for="i in 100" :key="i" :img="`https://picsum.photos/300/200?random=${i}`" :text="`Box ${i}`" />
    </div>
  </q-page>
</template>

<script lang="ts" setup>
import HelloWorld from '../components/HelloWorld.vue'
import Box from '../components/Box.vue'
</script>
