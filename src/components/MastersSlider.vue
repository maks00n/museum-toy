<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Navigation, Pagination } from 'swiper/modules'
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
]
</script>

<template>
  <div class="masters-slider">
    <h2 class="masters-slider__title">НАШИ МАСТЕРА</h2>
    <Swiper
      :modules="[Navigation, Pagination]"
      :slides-per-view="4"
      :space-between="20"
      :loop="true"
      class="masters-slider__swiper"
    >
      <swiper-slide v-for="master in masters" :key="master.id">
        <MastersCard :surname="master.surname" :name="master.name" :image="master.image" />
      </swiper-slide>
    </Swiper>
  </div>
</template>

<style lang="scss" scoped>
.masters-slider {
  width: 1784.73rem;
  margin: 300rem auto 0;
  position: relative;

  &__title {
    font-family: 'Arial';
    font-size: 140rem;
    font-weight: 600;
    color: #8050162e;
    position: absolute;
    top: -30rem;
    left: 0;
  }

  &__swiper {
    ::v-deep .swiper-button-next,
    ::v-deep .swiper-button-prev {
      color: $primary-color;
    }

    ::v-deep .swiper-pagination-bullet {
      background: $primary-color;
      opacity: 0.5;

      &-active {
        opacity: 1;
      }
    }
  }
}
</style>
