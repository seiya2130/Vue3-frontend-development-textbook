<script setup lang="ts">
import {ref} from "vue";

const url = ref("http://vuejs.org/")


</script>

<template>
  <p>
    <a v-bind:href="url" target="_blank">Vue.jsのサイト</a>
    <a :href="url" target="_blank">Vue.jsのサイト</a>
    <a v-bind:href="url + 'guide/introduction.html'" target="_blank">Vue.jsガイドのページ</a>
  </p>
</template>