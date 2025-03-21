<template>
  <q-page class="no-padding">
    <!-- Banner Section -->
    <section class="section-banner">
      <BannerComponent />
    </section>
    <section class="section-cards">
      <CardComponent />
    </section>
  </q-page>
</template>

<script setup>
import BannerComponent from 'src/components/BannerComponent.vue'
import CardComponent from 'src/components/CardComponent.vue'
</script>

<style scoped lang="scss">
.section-banner {
  height: 100vh;
}

.section-cards {
  max-width: 1300px;
  margin: 0 auto;
}
</style>
