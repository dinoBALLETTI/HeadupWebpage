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

<!-- *** MOBILE GROUP *** -->
    <div class="social-media__container--mobile">
        <img :src="LinkedInIcon">
        <img :src="YoutubeIcon">
    </div>

    <div class="link__container--mobile">
        <a>Plateforme Head Up </a>
        <a>Ateliers de formation</a>
        <a>Qui sommes-nous ? </a>
        <a>Blog</a>
        <a>CGU</a>
        <a>Politique de confidentialité</a>
        <a>Gestion des cookies</a>
        <a>Mentions légales</a>
    </div>

<!-- *** DESKTOP GROUP *** -->
    <div class="links__solution">
        <a class="title">Solution</a>
        <a>Plateforme Head Up </a>
        <a>Ateliers de formation</a>
    </div>
    
    <div class="links__about">
        <a class="title">A propos</a>
        <a>Qui sommes-nous ? </a>
        <a>Blog</a>
    </div>
    
    <div class="links__social">
        <a class="title">Follow Us</a>
        <img :src="LinkedInIcon">
        <img :src="YoutubeIcon">
    </div>

    <div class="divider"></div>

    <div class="slogan__container">
        <div class="slogan--left-container">
            <a>Copyright © 2023 Head Up | Révèle le potentiel de vos salariés</a>
        </div>
        <div class="slogan--right-container">
            <a>CGU</a>
            <a>Politique de confidentialité</a>
            <a>Gestion des cookies</a>
            <a>Mentions légales</a>
        </div>
    </div>

</div>
</template>

<style scoped>
.footer__container {
    display:grid;
    gap: 16px;
    grid-template-columns: 1;
    grid-template-rows: 4;
    padding: 48px 35px;
    width: 100%;
}
.social-media__container--mobile {
    grid-column: 1;
    grid-row: 2;
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
    grid-column: 1;
    grid-row:1;
    line-height: normal;
    max-width: 400px;
}
.link__container--mobile {
    align-items: flex-start;
    color: var(--Black, #000);
    display: flex;
    flex-direction: column;
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    gap: 4px;
    grid-column: 1;
    grid-row: 3;
    line-height: normal;
}
.links__solution {
    display: none;
}
.links__about {
    display: none;
}
.links__social {
    display: none;
}
.divider {
    align-self: stretch;
    background: var(--Black, #000);
    grid-column: 1;
    grid-row: 4;
    height: 1.05px;
    width: 100%;
}
.slogan__container {
    grid-column: 1;
    grid-row: 4;
}
.slogan--right-container {
    display: none;
}
.slogan--left-container {
    color: var(--Black, #000);
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

@media screen and (min-width:600px) {
    .footer__container {
        gap: 40px;
        grid-template-columns: 50% repeat(3, 1fr);
        grid-template-rows: 2;
        padding: 80px 65px; 
    }
    .social-media__container--mobile {
        display: none;
    }
    .link__container--mobile {
        display: none;
    }
    .links__solution {
        grid-column: 2;
        grid-row: 1;
    }
    .links__about {
        grid-column: 3;
        grid-row: 1;
    }    
    .links__social {
        grid-column: 4;
        grid-row: 1;
    }
    [class^='links__'] {
        align-items: flex-start;
        display: flex;
        flex-direction: column;
        flex: 1 0 0;   
        gap: 17px;
    }
    .title {
        color: var(--Black, #000);
        font-family: Open Sans;
        font-size: 16.732px;
        font-style: normal;
        font-weight: 600;
        line-height: 150%;
    }
    [class^='links__'], a {
        color: var(--Black, #000);
        font-family: Open Sans;
        font-size: 14.641px;
        font-style: normal;
        font-weight: 400;
        line-height: 150%;
    }
    .divider {
        grid-column: 1 / 5;
        grid-row: 2;
    }
    .slogan__container {
        display: flex;
        grid-column: 1 / 5;
        grid-row: 2;
        justify-content: space-between;
        padding-top: 20px;
    }
    .slogan--right-container {
        display: flex;
        flex-direction: row;
        gap: 25px;
    }
}
</style>