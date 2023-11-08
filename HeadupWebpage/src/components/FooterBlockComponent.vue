<script setup>
import LinkedInIcon from '@/assets/icons/linkedIn.svg';
import YoutubeIcon from '@/assets/icons/youtube.svg';
import TextInputItem from '../components/shared/TextInputItem.vue'
</script>

<template>
<div class="footer__container">

    <div class="newsletter__container">
        <img src="../assets/medias/Logo.png" style="padding-bottom: 8px;">
        <p>Ne ratez aucun de nos articles ! </p>
        <div class="newsletter__input">

            <TextInputItem :text="'Votre e-mail professionnel'" />
        </div>
    </div>

    <div class="social-media__container">
        <img :src="LinkedInIcon">
        <img :src="YoutubeIcon">
    </div>

    <div class="links__container">
        <p>Plateforme Head Up </p>
        <p>Ateliers de formation</p>
        <p>Qui sommes-nous ? </p>
        <p>Blog</p>
        <p>CGU</p>
        <p>Politique de confidentialité</p>
        <p>Gestion des cookies</p>
        <p>Mentions légales</p>
    </div>

    <div class="divider"></div>

    <div class="slogan">
        <a>Copyright © 2023 Head Up | Révèle le potentiel de vos salariés</a>
    </div>

</div>
</template>

<style scoped>
.footer__container {
    display: grid;
    width: 100%;
    padding: 48px 35px;
    gap: 16px;
}
.newsletter__container {
    align-items: flex-start;
    align-self: stretch;
    color: var(--Black, #000);
    display: flex;
    flex-direction: column;
    flex-shrink: 0;
    font-family: Open Sans;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    gap: 16px;
    line-height: normal;
}
.newsletter__input {
    width: min(100%, 400px)
}
.social-media__container {
    display: flex;
    align-items: center;
}
.links__container p{
    color: var(--Black, #000);
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.divider {
    align-self: stretch;
    background: var(--Black, #000);
    height: 1.05px;
}

.slogan a {
    color: var(--Black, #000);
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
</style>