<template>
  <div class="card-container">
    <img :src="fullImgageUrl" :alt="altText" class="image" />
    <div class="container">
      <h2>{{ heading }}</h2>
      <span>{{ date }}</span>
      <p class="description">
        {{ description }}
      </p>
      <span class="read-more">Read more...</span>
    </div>
  </div>
</template>

<script setup lang="ts">
import { computed } from "vue";

const fullImgageUrl = computed(() => {
  // return new URL(`../assets/img/${props.imageSrc}`, import.meta.url).href;
  return new URL(`../assets/img/${props.imageSrc}`, import.meta.url).href;
});

const props = defineProps({
  imageSrc: String,
  altText: String,
  heading: String,
  date: String,
  description: String,
});
</script>

<style scoped>
.card-container {
  background-color: wheat;
  padding: 1rem;

  display: flex;
  gap: 1rem;
}

.image {
  object-fit: cover;
  width: 230px;
  height: 230px;
}

.container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.description {
  overflow: hidden;

  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 4;
  line-clamp: 4;
}
</style>
