<template>
  <div class="justify-center align-center" :class="classContainerCard">
    <q-card class="my-card" flat bordered>
      <q-card-section horizontal>
        <q-card-section>
          <div :class="classOverline">{{ overline }}</div>
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
defineProps({
  classContainerCard: {
    type: String,
    default: 'container-card',
  },
  classOverline: {
    type: String,
    default: 'text-overline text-accent',
  },
  overline: {
    type: String,
    default: 'Overline',
  },
  title: {
    type: String,
    default: 'Title',
  },
  lorem: {
    type: String,
    default: `Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.`,
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
</script>

<style scoped lang="scss">
.container-card {
  max-width: 1300px;
  margin: 0 auto;
}
</style>
