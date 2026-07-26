<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 136****4411 完成了悬疑电影雨夜酒吧分景美术方案"
  },
  {
    "text": "用户 188****7720 生成了民国剧情片主卧灯光机位布置"
  },
  {
    "text": "用户 132****9988 完成了古风短剧竹林客栈低成本置景清单"
  },
  {
    "text": "用户 153****1155 生成了带货直播间 4 灯法布光与背景软装"
  },
  {
    "text": "用户 177****6633 取得了科幻废土风格虚拟制片分景图册"
  }
]);
</script>
