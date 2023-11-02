<template>
    <div class="cta__ctnr">
        <div class="cta__content">
        <h2>Envie d’utiliser la préparation mentale pour vos équipes ?</h2>
        <h3>Echangeons 20 minutes pour vous présenter nos solutions d’accompagnement et la plateforme Head Up. </h3>
        <ButtonItem :text="'Contactez-nous !'" :link="'your-demo-link'"/>
        </div>
    </div>
</template>

<script setup>
import ButtonItem from './shared/ButtonItem.vue';
</script>

<style scoped>
.cta__ctnr {
    display: flex;
    align-items: flex-start;
    background-position: center;
    background-size: cover;
    background: linear-gradient(0deg, rgba(9, 170, 151, 0.49) 0%, rgba(9, 170, 151, 0.49) 100%), url(../assets/medias/ctaBanner.png), lightgray 50%;
    flex-direction: column;
    justify-content: center;
    padding: 48px 35px;
    width: 100%;
}
.cta__content{
    align-items: flex-start;
    color: white;
    display: flex;
    flex-direction: column;
    gap: 16px; 
    justify-content: center;
    width: 100%;
}
.cta__content h2 {
    align-self: stretch;
    font-size: 24px;
}

.cta__content h3 {
    font-size: 16px;
}

@media screen and (min-width: 600px) {
    .cta__ctnr {
        padding: 100px 65px; 

    }
    .cta__content {
        max-width: 680px;
    }
    .cta__content h2 {
        font-size: 32px;
    }
    .cta__content h3 {
        font-size: 18px;
    }
}
</style>