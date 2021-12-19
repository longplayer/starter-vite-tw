<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <p>
    <a href="https://www.npmjs.com/package/vite-aliases" target="_blank">
      vite-aliases Documentation
    </a>
    |
    <a href="https://vitejs.dev/guide/using-plugins.html" target="_blank">Vue 3 Adding plugin Docummentation</a>
  </p>

  <div class="bg-gray-100 w-6/12 p-4 mx-auto my-8 rounded">
    <button class="rounded p-4 bg-green-600 text-white" type="button" @click="state.count++">count is: {{ state.count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test hot module replacement.
    </p>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
