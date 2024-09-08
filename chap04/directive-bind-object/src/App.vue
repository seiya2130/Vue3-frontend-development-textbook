<script setup lang="ts">
import {ref} from "vue";

const pBgColor = ref("white");
const onPClick = (bgClolor: string): void => {
  pBgColor.value = bgClolor;
}

</script>

<template>
  <p v-on:click="onPClick('red')" v-bind:style="{backgroundColor: pBgColor}">クリックする</p>
</template>

