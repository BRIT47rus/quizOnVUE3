<template>
  <button aria-label="умненьшить количество" type="button" :class="{ buttonEnter: isEnternBTN }">
    <BaseIcon v-if="iconSvg" :name="iconSvg" />
    <span v-else>{{ text }}</span>
  </button>
</template>

<script setup>
import BaseIcon from '@/components/BaseIcon.vue';
const props = defineProps({
  iconSvg: { type: String, default: '' },
  text: { type: String, default: '' },
  custemClass: { type: String, default: '' },
  isEnternBTN: { type: Boolean, default: false },
});
// const iconName = 'minusIcon';
</script>

<style scoped>
.base {
  background: red;
}
.buttonEnter {
  background-color: var(--secondary-200);
}
</style>
