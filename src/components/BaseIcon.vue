<template>
  <span v-if="iconSvg" v-html="iconSvg"></span>
  <img v-else-if="iconPath" :src="iconPath" alt="" />
  <span v-else>{{ text }}</span>
</template>

<script setup>
import { iconsMap } from '@/assets/utils/icons';
import { computed } from 'vue';

const props = defineProps({
  name: { type: String, default: '' },
  text: { type: String, default: '' },
});

const iconSvg = computed(() => {
  const icon = iconsMap[props.name];
  return typeof icon === 'string' && icon.trim().startsWith('<svg') ? icon : null;
});

const iconPath = computed(() => {
  const icon = iconsMap[props.name];
  return typeof icon === 'string' && !icon.trim().startsWith('<svg') ? icon : null;
});
</script>

<style scoped></style>
