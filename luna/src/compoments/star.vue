<script setup lang="ts"></script>
<template>
  <div class="big-dipper">
    <div class="star dubhe"></div>
    <div class="star merak"></div>
    <div class="star phecda"></div>
    <div class="star megrez"></div>
    <div class="star alioth"></div>
    <div class="star mizar"></div>
    <div class="star alkaid"></div>
  </div>
</template>
<style scoped>
/* ✨ 北斗七星區域 */
.big-dipper {
  position: absolute;
  bottom: 0%;
  left: 50%;
  width: 400px;
  height: 200px;
  transform: translateX(-50%);
}

/* 共用的星星樣式 */
.star {
  position: absolute;
  width: 8px;
  height: 8px;
  background: white;
  border-radius: 50%;
  box-shadow: 0 0 10px 3px white;
  animation: twinkle 2s ease-in-out infinite alternate;
}

/* ✳️ 每顆星的位置（模擬北斗七星形狀，勺身從右邊開始） */
.dubhe {
  left: 94%;
  top: 20%;
  animation-delay: 0s;
} /* 天樞 - 勺身起點，右上方 */
.merak {
  left: 91%;
  top: 57%;
  animation-delay: 0.2s;
} /* 天璇 - 勺身下方 */
.phecda {
  left: 63%;
  top: 61%;
  animation-delay: 0.4s;
} /* 天玑 - 勺身底部 */
.megrez {
  left: 58%;
  top: 30%;
  animation-delay: 0.6s;
} /* 天權 - 勺身與勺柄的連接點 */
.alioth {
  left: 40%;
  top: 17%;
  animation-delay: 0.8s;
} /* 玉衡 - 勺柄起點 */
.mizar {
  left: 26%;
  top: 5%;
  animation-delay: 1s;
} /* 開陽 - 勺柄中間 */
.alkaid {
  left: 2%;
  top: 16%;
  animation-delay: 1.2s;
} /* 搖光 - 勺柄末端，左上方 */

/* ⭐ 閃爍動畫 */
@keyframes twinkle {
  0%,
  100% {
    opacity: 0.9;
  }
  50% {
    opacity: 0.3;
  }
}
</style>
