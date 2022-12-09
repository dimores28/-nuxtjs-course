<template>
  <a href="#" @click="view('home')">Home</a>
  <a href="#" @click="view('counter')">Counter</a>

  <!-- <button @click="toggle">Toggle</button> -->
  <LazyHomeWelcome v-if="page === 'home'" />

  <!-- <component :is="MyComponent" /> -->
  <LazyCounter v-if="page === 'counter'" />
</template>

<script setup>
// const MyComponent = shallowRef(resolveComponent("Counter"));
const MyComponent = ref("counter");

function toggle() {
  MyComponent.value = "welcome";
}

const page = ref("home");

function view(name) {
  page.value = name;
}
</script>
