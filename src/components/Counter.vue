<template>
  <div className="counter">
    <PTag>Выбери количество вопросов:</PTag>
    <form action="">
      <button aria-label="умненьшить количество" type="button">
        <img src="/minus.svg" alt="" aria-hidden="true;" />
      </button>
      <input type="text" />
      <button aria-label="увеличить количество" type="button">
        <img src="/plus.svg" alt="" aria-hidden="true;" />
      </button>
    </form>
  </div>
</template>

<script setup>
import PTag from '@/components/PTag.vue';
</script>

<style scoped>
.counter {
  display: grid;
  gap: var(--spaccing-l);
}
</style>
