<template>
    <div class="cta_ctnr">
        <div class="ctaContent">
        <h2>Envie d’utiliser la préparation mentale pour vos équipes ?</h2>
        <h3>Echangeons 20 minutes pour vous présenter nos solutions d’accompagnement et la plateforme Head Up. </h3>
        <ButtonItem :text="'Réserver une démo'" :link="'your-demo-link'"/>
        </div>
    </div>
</template>

<script setup>
import ButtonItem from './shared/ButtonItem.vue';
</script>

<style scoped>
.cta_ctnr {
    display: flex;
width: 1513px;
padding: 100px 65px;
flex-direction: column;
justify-content: center;
align-items: flex-start;
gap: 84.107px; 
background: linear-gradient(0deg, rgba(9, 170, 151, 0.49) 0%, rgba(9, 170, 151, 0.49) 100%), url(../assets/medias/ctaBanner.png), lightgray 50% / cover no-repeat;
background-position: center;
background-size: 100%;
}
.ctaContent{
    display: flex;
width: 680px;
flex-direction: column;
justify-content: center;
align-items: flex-start;
gap: 25.232px; 
color: white;
}
</style>