<template>
  <div>
    <nav>
      <NuxtLink to="/">Home</NuxtLink>
      <NuxtLink to="about">About</NuxtLink>
      <NuxtLink to="profile">Profile</NuxtLink>
    </nav>

    <!-- here nuxt replace page content -->
    <slot></slot>
  </div>
</template>

<style scoped>
a {
  margin: 10px;
}
</style>
