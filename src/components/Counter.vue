<script setup>
import { ref } from 'vue';
import PTag from '@/components/PTag.vue';
import ButtonCustom from '@/components/ButtonCustom.vue';

const iconMinus = 'minusIcon';
const iconPlus = 'plusIcon';
</script>

<template>
  <div class="counter">
    <PTag>Выбери количество вопросов:</PTag>
    <form className="form">
      <ButtonCustom :iconSvg="iconMinus" />
      <div className="input">
        <input type="text" autofocus />
      </div>
      <ButtonCustom :iconSvg="iconPlus" />
    </form>

    <ButtonCustom text="Начать" isEnternBTN="false" />
  </div>
</template>

<style scoped>
.counter {
  display: grid;
  justify-content: center;
  align-items: center;
  gap: var(--spaccing-l);
}
.form {
  display: flex;
  justify-content: center;
  gap: var(--gap-m);
}
.input {
  border: 4px solid var(--primari-200);
  width: 118px;
  height: 76px;
  border-radius: var(--brs);
  input {
    text-align: center;
    width: 100%;
    height: 100%;
    font-size: 36px;
  }
}
</style>
