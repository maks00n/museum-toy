<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Navigation } from 'swiper/modules'
import FiguresCard from './FiguresCard.vue'

import 'swiper/css'
import 'swiper/css/navigation'
import 'swiper/css/pagination'

// заглушка
const figures = [
  {
    id: 1,
    image: '/figures/figure1.jpg',
    name: 'Ангел',
    description:
      'Фигура ангела является символом защиты и духовной поддержки. Она стоит рядом с семьей, напоминая о невидимом влиянии, которое следит за вами и вашими близкими. Орнаменты на нимбе и крыльях ангела добавляют уникальности этой композиции, придавая ей особое визуальное очарование.',
  },
  { id: 2, image: '/figures/figure2.jpg', name: 'Рисунок 2', description: 'Описание 2' },
  { id: 3, image: '/figures/figure3.jpg', name: 'Рисунок 3', description: 'Описание 3' },
  { id: 4, image: '/figures/figure4.jpg', name: 'Рисунок 4', description: 'Описание 4' },
  { id: 5, image: '/figures/figure5.jpg', name: 'Рисунок 5', description: 'Описание 5' },
]
</script>

<template>
  <div class="figures-slider">
    <Swiper
      :modules="[Navigation]"
      :navigation="{
        prevEl: '.swiper-button-prev-custom',
        nextEl: '.swiper-button-next-custom',
      }"
      :slides-per-view="1"
      :loop="true"
      class="swiper"
    >
      <swiper-slide v-for="figure in figures" :key="figure.id">
        <FiguresCard :image="figure.image" :name="figure.name" :description="figure.description" />
      </swiper-slide>
    </Swiper>
    <div class="swiper-button-prev-custom">
      <img src="@/assets/images/arrow-left.svg" alt="prev" />
    </div>
    <div class="swiper-button-next-custom">
      <img src="@/assets/images/arrow-right.svg" alt="next" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.figures-slider {
  width: 1738.48rem;
  margin: 150rem auto 0;
  position: relative;

  .swiper-button-prev-custom,
  .swiper-button-next-custom {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;
    z-index: 10;
  }

  .swiper-button-prev-custom {
    left: 0;
    img {
      width: 100rem;
    }
  }

  .swiper-button-next-custom {
    right: 0;
    img {
      width: 100rem;
    }
  }
}
</style>
