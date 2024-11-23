<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import TopHeader from '@/components/TopHeader.vue'
</script>

<template>
  <TopHeader />
  <RouterView />
</template>

<style lang="scss">
@use './assets/style.scss' as *;
</style>
