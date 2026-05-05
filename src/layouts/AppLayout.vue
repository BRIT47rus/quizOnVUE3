<template>
  <div className="app">
    <Header />
    <Card>
      <WellcomeView />
    </Card>
    <Footer />
  </div>
</template>
<script setup>
import Card from '@/components/Card.vue';
import WellcomeView from '@/views/WellcomeView.vue';
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
</script>

<style scoped>
.app {
  display: grid;
  grid-template-rows: 48px 1fr 16px;
  grid-template-columns: minmax(343px, 590px);
  gap: var(--gap-m);
}
</style>
