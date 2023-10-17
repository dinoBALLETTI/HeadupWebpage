<template>
<div class="partners_ctnr">
    <h2>Nos partenaires de confiance</h2>
    <div class="partners_carousel">
        <Carousel />
    </div>
</div>
</template>

<script setup>
import Carousel from '@/components/shared/Carousel.vue'
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