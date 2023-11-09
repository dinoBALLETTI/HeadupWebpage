<script setup>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Navigation } from 'vue3-carousel'
import {slides} from '../data/PartnersData.vue';

const breakpoints = {
  // 700px and up
  700: {
    itemsToShow: 3,
    snapAlign: 'center',
  },
  // 1024 and up
  1024: {
    itemsToShow: 4,
    snapAlign: 'start',
  },
}
</script>

<template>
    <Carousel 
      :wrap-around="true" 
      :breakpoints="breakpoints" 
      :autoplay="2000"
      :pauseAutoplayOnHover="true"
    >
      <Slide v-for="slide in slides" :key="slide.id">
        <div class="carousel__item">
          <img :src="slide.source">
        </div>
      </Slide>
  
      <template #addons>
        <Navigation />
      </template>
    </Carousel>

</template>


<style>
.carousel__item {
  max-height: 256px;
  width: 100%;
  padding: 0px 20px 0px 20px ;
  justify-content: center;
  align-items: center;

}

.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}

</style>