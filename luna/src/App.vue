<script setup lang="ts">
import Moon from './compoments/moon.vue'
import Star from './compoments/star.vue'
import Title from './compoments/title.vue'
</script>

<template>
  <div class="luna">
    <Moon />
    <Title />
    <Star />
  </div>
</template>

<style scoped>
.luna {
  background-image: url('https://thumb.photo-ac.com/ba/babecdc7df4e970cc8889a3255c119c4_t.jpeg');
  background-size: cover;
  width: 100%;
  height: 100%;
  position: relative;
  max-width: 600px;
  margin: 0 auto;
}
</style>
