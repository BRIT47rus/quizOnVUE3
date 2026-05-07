<template>
  <button aria-label="умненьшить количество" type="button" v-bind="icon">
    <BaseIcon :name="iconName" :text="text" />
  </button>
</template>

<script setup>
import BaseIcon from '@/components/BaseIcon.vue';
const props = defineProps({
  iconSvg: { type: String, default: '' },
  text: { type: String, default: '' },
});
// const iconName = 'minusIcon';
</script>

<style scoped></style>
