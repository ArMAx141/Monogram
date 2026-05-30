<template>
  <div class="navbar-container">
    <h1>Navbar</h1>
    <ul class="nav-links-container">
      <li>Home</li>
      <li>About</li>
      <li>Contact</li>
      <li>User</li>
    </ul>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.navbar-container {
  background-color: rgb(182, 171, 117);

  display: flex;
  justify-content: space-between;

  padding: 1rem;
}

.nav-links-container {
  list-style: none;
  display: flex;
  align-items: center;
  gap: 2rem;
  margin-right: 1rem;
}
</style>
