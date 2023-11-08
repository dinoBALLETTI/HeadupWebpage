<script setup>
import bpiLogo from '@/assets/medias/bpiLogo.png';
import esiaLogo from '@/assets/medias/esiaLogo.png';
import esjLogo from '@/assets/medias/esjLogo.png';
import gojoLogo from '@/assets/medias/gojoLogo.png';
import p27Logo from '@/assets/medias/p27Logo.png';
import ressourcupLogo from '@/assets/medias/ressourcupLogo.png';
import ttcLogo from '@/assets/medias/ttcLogo.png';
</script>

<template>

<div class="carousel  w-full">

  <div id="slide1" class="carousel-item relative w-full">
    <img :src="bpiLogo" class="p-15 w-full" />
  </div> 
  
  <div id="slide2" class="carousel-item relative w-full">
    <img :src="esiaLogo" class="p-15 w-full" />
  </div> 

  <div id="slide3" class="carousel-item relative w-full">
    <img :src="esjLogo" class="p-15 w-full" />
  </div> 

  <div id="slide4" class="carousel-item relative w-full">
    <img :src="gojoLogo" class="p-15 w-full" />
  </div>

  <div id="slide5" class="carousel-item relative w-full">
    <img :src="p27Logo" class="w-full" />
  </div>

  <div id="slide6" class="carousel-item relative w-full">
    <img :src="ressourcupLogo" class="w-full" />
  </div>

  <div id="slide7" class="carousel-item relative w-full">
    <img :src="ttcLogo" class="w-full" />
  </div>

</div>

</template>

<style scoped>
.carousel {
  width: 100%;
}
</style>
