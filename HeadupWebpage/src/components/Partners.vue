<template>
    <div class="partners_ctnr">
        <h2>Nos partenaires de confiance</h2>
<div class="partners_carousel">

    <div v-for="partner in partners" :key="partner">
        <CarouselCard :partner=partner />
    </div>
        </div>
    </div>
</template>

<script setup>
import CarouselCard from './shared/CarouselCard.vue';
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
<style scoped>
.partners_ctnr{
    background: var(--White, #FFF);
}
.partners_carousel{
    display: flex;
    flex-direction: row;

}
</style>