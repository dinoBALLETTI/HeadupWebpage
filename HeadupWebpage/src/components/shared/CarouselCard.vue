<template>
    <div class="card_ctnr"><img :src="partner"></div>
  </template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps(['partner'])
</script>

<style scoped>
.card_ctnr {
    width: 300px;
    height: 300px;
}
.card_ctnr img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>