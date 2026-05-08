<template>
  <button
    aria-label="умненьшить количество"
    type="button"
    class="base"
    :class="{ buttonEnter: isEnternBTN }"
  >
    <BaseIcon v-if="iconSvg" :name="iconSvg" />
    <span v-else>{{ text }}</span>
  </button>
  <span v-if="isEnternBTN" class="enterText">или нажми Enter ↵</span>
</template>

<script setup>
import BaseIcon from '@/components/BaseIcon.vue';
const props = defineProps({
  iconSvg: { type: String, default: '' },
  text: { type: String, default: '' },
  custemClass: { type: String, default: '' },
  isEnternBTN: { type: Boolean, default: false },
});
</script>

<style scoped>
.base {
  display: flex;
  justify-content: center;
  align-items: center;
}
.buttonEnter {
  width: 100%;
  margin: 0 auto;
  border-radius: var(--brs);
  padding: var(--spase-padd-m);
  color: var(--bg);
  font-size: var(--font-span-x-size);
  font-weight: var(--font-h-weigth);
  max-width: 270px;
  background-color: var(--secondary-200);
}
.enterText {
  text-align: center;
  font-size: var(--font-span-s-size);
  line-height: var(--font-span-s-lh);
  margin-top: -8px;
}
</style>
