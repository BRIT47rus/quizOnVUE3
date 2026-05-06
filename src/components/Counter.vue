<script setup>
import PTag from '@/components/PTag.vue';
</script>

<template>
  <div className="counter">
    <PTag>Выбери количество вопросов:</PTag>
<Button/>
    <form className="form">
<Button/
      <div className="input">
        <input type="text" />
      </div>
      <button aria-label="увеличить количество" type="button">
        <img src="/plus.svg" alt="" aria-hidden="true;" />
      </button>
    </form>
  </div>
</template>

<style scoped>
.counter {
  display: grid;
  gap: var(--spaccing-l);
}
.form {
  display: flex;
}
.input {
  border: 4px solid var(--primari-200);
  width: 118px;
  height: 76px;
  input {
    border: none;
    outline: none;
    width: 100%;
    height: 100%;
    font-size: 36px;
  }
}
</style>
