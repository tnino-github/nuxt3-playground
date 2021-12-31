<script setup lang="ts">
const counter = ref(0)
const doubled = computed(() => counter.value * 2)
const increment = () => {
  counter.value++
  return { counter, doubled, increment }
}
</script>

<template>
  <div>
    <p>{{ counter }}</p>
    <p>{{ doubled }}</p>
    <p><button @click="increment">カウントアップ</button></p>
  </div>
</template>
