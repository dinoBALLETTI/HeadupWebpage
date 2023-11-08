<script setup>
import VueCarouselItem from './shared/VueCarouselItem.vue';
</script>

<template>

<div class="partners__container">
    <div class="partners">Nos partenaires de confiance</div>
        <div class="carousel__container">
            <VueCarouselItem />
        </div>
</div>
</template>
<style scoped>
.partners {
    color: var(--grises-darkest, var(--Grises-darkest, #20282C));

/* Desktop H2 - Heading 2 */
font-family: Poppins;
font-size: 32px;
font-style: normal;
font-weight: 700;
line-height: normal;
}
.partners__container {
    display: flex;
width: 100%;
padding: 100px 65px;
flex-direction: column;
justify-content: center;
align-items: center;
gap:50px;
}

div.carousel__container {
    width:100%;
}
</style>