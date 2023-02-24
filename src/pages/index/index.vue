<template>
  <view class="content">
    <!-- <image class="logo" src="/static/logo.png" /> -->
    <FlipClock class="cls-clock-container" />
  </view>
</template>

<script setup lang="ts">
import FlipClock from '@/components/flip-clock/FlipClock.vue';
import { ref } from 'vue'
const title = ref('Hello')
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.cls-clock-container {
  font: normal 14px "Helvetica Neue", Helvetica, sans-serif;
  user-select: none;
  text-shadow: 0 1px 0 rgba(0, 0, 0, 0.3);
  background: radial-gradient(ellipse at center, #969696 0%, #595959 100%);
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin-top: 200rpx;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50rpx;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
