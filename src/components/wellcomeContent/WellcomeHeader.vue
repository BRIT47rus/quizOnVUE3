<template>
  <div className="welcome-header">
    <p className="title">Добро пожаловать</p>
    <PTag>на викторину по странам и столицам!</PTag>
  </div>
</template>

<script setup>
import PTag from '@/components/PTag.vue';
</script>

<style scoped>
.welcome-header {
  text-align: center;
}
.title {
  font-size: var(--font-h-size);
  line-height: var(--font-h-lh);
  font-weight: var(--font-h-weigth);
}
</style>
