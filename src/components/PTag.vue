<template>
  <p className="subTitle"><slot></slot></p>
</template>

<script setup></script>

<style scoped>
.subTitle {
  font-size: var(--font-p-size);
  line-height: var(--font-p-lh);
}
</style>
