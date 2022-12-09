<template>
  <div>
    <h1>Hello Index</h1>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="about">About</NuxtLink>

    <button @click="movetoAbout">Take me to About Page</button>
  </div>
</template>

<script setup>
function movetoAbout() {
  navigateTo("about");
}
</script>
