<template>
    <div v-for="partner in partners" :key="partner">
        <CarouselCard :partner="partner" />
    </div>
</template>

<script setup>
import CarouselCard from './CarouselCardItem.vue';
import bpiLogo from '@/assets/medias/bpiLogo.png';
import esiaLogo from '@/assets/medias/esiaLogo.png';
import esjLogo from '@/assets/medias/esjLogo.png';
import gojoLogo from '@/assets/medias/gojoLogo.png';
import p27Logo from '@/assets/medias/p27Logo.png';
import ressourcupLogo from '@/assets/medias/ressourcupLogo.png';
import ttcLogo from '@/assets/medias/ttcLogo.png';

const partners = [
    bpiLogo,
    esiaLogo,
    esjLogo,
    gojoLogo,
    p27Logo,
    ressourcupLogo,
    ttcLogo
]
</script>