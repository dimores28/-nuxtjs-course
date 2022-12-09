<template>
  <main class="user-layout">
    <article class="sidebar">
      <p>Dashboard</p>
      <p>Settings</p>
    </article>
    <section>
      <!-- here nuxt replace page content -->
      <slot></slot>
    </section>
  </main>
</template>

<style scoped>
.user-layout {
  display: flex;
}
.sidebar {
  display: flex;
  flex-direction: column;
}
</style>
