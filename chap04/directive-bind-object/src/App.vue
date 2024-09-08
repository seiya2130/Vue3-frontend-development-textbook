<script setup lang="ts">
import {ref} from "vue";

const mousePointX = ref(0)
const mousePointY = ref(0)

const onImgMousemove = (event: MouseEvent): void => {
  mousePointX.value = event.offsetX;
  mousePointY.value = event.offsetY;
}
</script>

<template>
  <section>
    <img src="./assets/logo.svg" alt="ロゴ" width="200" v-on:mousemove="onImgMousemove">
    <p>ポインタの位置 x={{ mousePointX }}; y={{ mousePointY }}</p>
  </section>
</template>