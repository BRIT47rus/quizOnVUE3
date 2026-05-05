<template>
  <footer className="footer">
    <span>
      Проект выполнен в рамках стажировки&nbsp;
      <a
        href="https://preax.ru"
        rel="noopener noreffer"
        target="_blank"
        className="link"
        aria-label="Переход на сайт Preax"
      >
        PREAX
      </a>
    </span>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer {
  display: flex;
  align-items: end;
  font-size: 14px;
  color: var(--color-bg);
  font-weight: var(--font-span-m-weigth);
  @media (width < 768px) {
    & {
      font-size: 10px;
    }
  }
}
.link {
  text-decoration: underline;
  text-underline-offset: 3px;
}
</style>
