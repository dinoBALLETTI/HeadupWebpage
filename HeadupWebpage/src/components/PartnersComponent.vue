  <script setup>
import MobileCarouselItem from '@/components/shared/MobileCarouselItem.vue';
import DesktopCarouselItem from './shared/DesktopCarouselItem.vue';
</script>

<template>

<!-- *** MOBILE GROUP *** -->
<div class="partners--mobile">

    <h2>Nos partenaires</h2>

    <div class="partners__carousel--mobile">
        <MobileCarouselItem />
    </div>

</div>

<!-- *** DESKTOP GROUP *** -->
<div class="partners--desktop">

    <h2>Nos partenaires de confiance</h2>

    <div class="partners__carousel--desktop">
        <DesktopCarouselItem />
    </div>

</div>

</template>
<style scoped>
.partners--mobile {
    display: flex;
    width: 100%;
    padding: 48px 35px 24px 35px;
    flex-direction: column;
    align-items: center;
    flex-shrink: 0;
}
.partners__carousel--mobile {
    padding: 0px 35px;
    align-items: center;
}
.partners--mobile h2 {
    color: var(--grises-darkest, var(--Grises-darkest, #20282C));
    text-align: center;
    font-family: Poppins;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    padding-bottom: 18px;
}

.partners--desktop {
    display: none;
    width: 100%x;
    padding: 100px 65px;
    flex-direction: column;
    align-items: center;
    gap: 50px;
}
.partners__carousel--desktop {
    padding: 0px 35px;
    align-items: center;
}
.partners--desktop h2 {
    color: var(--grises-darkest, var(--Grises-darkest, #20282C));
    font-family: Poppins;
    font-size: 32px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

@media screen and (min-width: 600px) {
    .partners--mobile {
        display: none;
    }
    .partners--desktop {
        display: flex
    }
}
</style>