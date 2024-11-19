<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
      <div>
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/contact">Contact</RouterLink>
          <RouterLink to="/products">Products</RouterLink>
        </nav>
      </div>
  </header>

  <main>
    <RouterView />
  </main>
</template>

<style scoped>

header {
  display: flex;
  
  padding: 2rem;
  background-color: rgb(211, 207, 207);
}

nav {
  display: flex;
  gap: 1rem;
  margin-bottom: 2rem;
}

main {
  width: min(100% - 4rem, 1000px);
  margin-inline: auto;
}

</style>