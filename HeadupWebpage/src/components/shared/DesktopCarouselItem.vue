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

<div class="carousel carousel-center rounded-box">
  <div class="carousel-item">
    <img :src="bpiLogo" />
  </div> 
  <div class="carousel-item">
    <img :src="esiaLogo" />
  </div> 
  <div class="carousel-item">
    <img :src="esjLogo" />
  </div> 
  <div class="carousel-item">
    <img :src="gojoLogo" />
  </div> 
  <div class="carousel-item">
    <img :src="p27Logo" />
  </div> 
  <div class="carousel-item">
    <img :src="ressourcupLogo" />
  </div> 
  <div class="carousel-item">
    <img :src="ttcLogo" />
  </div>
</div>

</template>

<style scoped>
.carousel {
    gap: 40px;
    width: 100%;
}
</style>
