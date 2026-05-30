<script setup lang="ts">
import navbar from "./components/navbar.vue";
import sidebar from "./components/sidebar.vue";
import "./assets/reset.css";
import card from "./components/card.vue";
</script>

<template>
  <div class="main-container">
    <navbar />
    <div class="container">
      <main>
        <card />
      </main>
      <sidebar />
    </div>
  </div>
</template>

<style scoped>
.main-container {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.container {
  display: flex;
  flex-direction: row;
  width: 100%;
  min-height: 100dvh;
  main {
    background-color: rgb(252, 249, 243);
    display: flex;
    flex-direction: column;
    gap: 1rem;
    width: 80%;
    padding: 1rem;
  }

  .aside-container {
    display: flex;
    flex-grow: 1;
  }
}
</style>

<!--
<template></template>

<script setup lang="ts"></script>

<style scoped></style>
  -->
