<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>
  <button type="button" @click="count++">Foo count is {{ count }}</button>
</template>

<style scoped>
button {
  background-color: crimson;
  color: white;
}
</style>
