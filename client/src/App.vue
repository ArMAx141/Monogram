<script setup lang="ts">
import navbar from "./components/navbar.vue";
import sidebar from "./components/sidebar.vue";
import "./assets/reset.css";
</script>

<template>
  <div class="main-container">
    <navbar />
    <div class="container">
      <main><h1>Main Content</h1></main>
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
    width: 80%;
    background-color: rgb(102, 135, 154);
    padding: 1rem;
  }

  .aside-container {
    display: flex;
    flex-grow: 1;
    background-color: rgb(154, 102, 102);
  }
}
</style>

<!--
<template></template>

<script setup lang="ts"></script>

<style scoped></style>
  -->
