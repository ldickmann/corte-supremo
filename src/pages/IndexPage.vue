<template>
  <q-page class="no-padding">
    <!-- Banner Section -->
    <section class="section-banner">
      <BannerComponent />
    </section>
    <CardComponent />
    <section class="section-black">
      <div class="container-services">
        <h2 class="text-h2 text-white text-center">Nossos Serviços</h2>
        <MiniCards />
      </div>
    </section>
  </q-page>
</template>

<script setup>
import BannerComponent from 'src/components/BannerComponent.vue'
import CardComponent from 'src/components/CardComponent.vue'
import MiniCards from 'src/components/MiniCards.vue'
</script>

<style scoped lang="scss">
.section-banner {
  height: 100vh;
}

.section-black {
  margin-top: 3rem;
  height: 60vh;
  background-color: $dark-page;

  .container-services {
    max-width: 1300px;
    margin: 0 auto;
    padding: 1rem 0;
    font-family: 'Hanken Grotesk';
  }
}
</style>
