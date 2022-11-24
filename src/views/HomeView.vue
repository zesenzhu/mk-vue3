<script setup lang="ts">
import { useCounterStore } from "../stores/counter";
const counter = useCounterStore();
const { count } = counter;
console.log(counter, count);
</script>

<template>
  <main>
    <p>{{ counter.count }}</p>
    <button @click="counter.increment">点击</button>
  </main>
</template>
