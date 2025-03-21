<template>
  <div class="q-pa-md row items-start q-gutter-md justify-center align-center">
    <q-card class="my-card" flat bordered>
      <q-card-section horizontal>
        <q-card-section>
          <div class="text-overline text-orange-9">Overline</div>
          <div class="text-h5 q-mt-sm q-mb-xs">{{ title }}</div>
          <div class="text-caption text-grey">
            {{ lorem }}
          </div>
        </q-card-section>

        <q-img class="col-7" :src="src" :alt="alt" />
      </q-card-section>
    </q-card>
  </div>
</template>

<script setup>
import { ref } from 'vue'

defineProps({
  title: {
    type: String,
    default: 'Title',
  },
  Overline: {
    type: String,
    default: 'Overline',
  },
  src: {
    type: String,
    default: 'images/image-1-card.jpg',
  },
  alt: {
    type: String,
    default: 'Imagem de um barbeiro cortando o cabelo de um cliente',
  },
})

const lorem = ref(
  'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
)
</script>

<style scoped lang="scss"></style>
