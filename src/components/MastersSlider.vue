<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Navigation, Autoplay } from 'swiper/modules'
import MastersCard from './MastersCard.vue'

import 'swiper/css'
import 'swiper/css/navigation'
import 'swiper/css/pagination'

// заглушка
const masters = [
  { id: 1, name: 'Анна', surname: 'Антонова', image: '/masters/anna.jpg' },
  { id: 2, name: 'Мария', surname: 'Максимова', image: '/masters/maria.jpg' },
  { id: 3, name: 'Елена', surname: 'Егорова', image: '/masters/elena.jpg' },
  { id: 4, name: 'Ольга', surname: 'Ольгина', image: '/masters/olga.jpg' },
  { id: 5, name: 'Наталья', surname: 'Натальева', image: '/masters/natalia.jpg' },
  { id: 6, name: 'Наталья', surname: 'Натальева', image: '/masters/natalia.jpg' },
]
</script>

<template>
  <div class="masters-slider">
    <h2 class="title">НАШИ МАСТЕРА</h2>
    <Swiper
      :modules="[Navigation, Autoplay]"
      :autoplay="{
        delay: 3000,
        disableOnInteraction: false,
      }"
      :slides-per-view="5"
      :space-between="20"
      :loop="true"
      class="swiper"
    >
      <swiper-slide v-for="master in masters" :key="master.id">
        <MastersCard :surname="master.surname" :name="master.name" :image="master.image" />
      </swiper-slide>
    </Swiper>
  </div>
</template>

<style lang="scss" scoped>
.masters-slider {
  width: 1699.2rem;
  margin: 300rem auto 0;
  position: relative;

  .title {
    font-family: 'Arial';
    font-size: 140rem;
    font-weight: 600;
    color: #8050162e;
    margin-left: -100rem;
  }
}
</style>
