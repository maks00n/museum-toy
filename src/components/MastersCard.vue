<script setup lang="ts">
defineProps<{
  surname: string
  name: string
  image: string
}>()
</script>

<template>
  <div class="masters-card">
    <img src="../assets/images/master.png" :alt="name" class="masters-card__image" />
    <span class="masters-card__surname">{{ surname }}</span>
    <span class="masters-card__name">{{ name }}</span>
  </div>
</template>

<style lang="scss" scoped>
.masters-card {
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;

  &__image {
    width: 387.68rem;
    height: 575.68rem;
    object-fit: cover;
    border-radius: 24rem;
  }

  &__surname {
    font-size: 40rem;
    line-height: 48rem;
    font-family: 'Condensed';
    color: $primary-color;
    margin-top: 39rem;
    text-transform: uppercase;
  }

  &__name {
    font-size: 16rem;
    margin-top: 9rem;
    text-transform: uppercase;
  }
}
</style>
