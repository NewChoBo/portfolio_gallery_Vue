<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })
const titleClass = ref('title')
</script>

<template>
  <h1 :class="titleClass">나를 빨갛게 만들어 보세요</h1>
  <p>숫자 세기: {{ counter.count }}</p>
</template>

<style>
.title {
  color: red;
}
</style>
