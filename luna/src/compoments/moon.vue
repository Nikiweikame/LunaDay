<script setup lang="ts"></script>
<template>
  <div class="moon">
    <img src="../assets/rabbit.png" alt="" />
  </div>
</template>
<style scoped>
.moon {
  height: 100px;
  width: 100px;
  background-image: url('../assets/moon.png');
  background-size: 150%;
  background-position-x: center;
  background-position-y: center;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 20%;
  right: 15%;
  transform: rotate(25deg);
  transform-origin: center center;

  animation: swing 2s ease-in-out infinite;
  transform-origin: center center; /* 從中心旋轉 */

  img {
    height: 90%;
  }
}
@keyframes swing {
  0% {
    transform: rotate(25deg);
  }
  50% {
    transform: rotate(35deg);
  }
  100% {
    transform: rotate(25deg);
  }
}
</style>
