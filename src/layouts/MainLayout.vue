<template>
  <q-layout view="hHh lpR fFf">
    <HeaderFloating />
    <q-page-container class="page-container">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup>
import HeaderFloating from 'src/components/HeaderFloating.vue'
</script>

<style scoped lang="scss">
.page-container {
  margin-top: -88px;
}
</style>
