<template>
  <button @click="increment">+</button>
  <p>{{ count }}</p>
  <button @click="decrement">-</button>
</template>

<script setup>
const count = ref(0);

function increment() {
  count.value++;
}

function decrement() {
  count.value--;
}
</script>
