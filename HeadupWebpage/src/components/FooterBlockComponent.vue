<script setup>
import ButtonItem from './shared/ButtonItem.vue';
import LinkedInIcon from '@/assets/icons/linkedIn.svg';
import YoutubeIcon from '@/assets/icons/youtube.svg';

</script>

<template>

        <div class="footer-ctnr">

        <div class="link-ctnr">

            <div class="newsletter-ctnr">
                <img src="../assets/medias/Logo.png">
                <p>Ne ratez aucun de nos articles ! </p>
                <input type="text">
                <ButtonItem :text="`M'inscrire`"/>
            </div>

            <div class="links">
                <a>Solution</a>
                <p>Plateforme Head Up </p>
                <p>Ateliers de formation</p>
            </div>

            <div class="links">
                <a>A propos</a>
                <p>Qui sommes-nous ?</p>
                <p>Blog</p>
            </div>
            
            <div class="links">
                <a>Suivez-nous</a>
                <img :src="LinkedInIcon" alt="LinkedIn Icon">
                <img :src="YoutubeIcon" alt="LinkedIn Icon">
            </div>
        </div>
        <div class="credits-ctnr">
            <div class="credits-divider"></div>
            <div class=credits-links>

                <span style="padding-right: 600px;">Copyright © 2023 Head Up | Révèle le potentiel de vos salariés</span>

                <div :href="link">
                    <div>CGU</div>
                </div>

                <div :href="link">
                <div>Politique de confidentialité</div>
                </div>

                <div :href="link">
                <div>Gestion des cookies</div>
                </div>

                <div :href="link">
                <div>Mentions légales</div>
                </div>

            </div>
        </div>
    </div>
</template>

<style scoped>
.footer-ctnr {
    display: flex;
width: 1512px;
height: 396px;
padding: 80px 65px;
flex-direction: column;
align-items: flex-start;
gap: 48px;}
.newsletter-ctnr {
    display: flex;
width: 522.879px;
flex-direction: column;
align-items: flex-start;
gap: 25.098px;
}
.link-ctnr{
    display:flex;
    flex-direction: row;
    gap: 41px
}
.links {
    display: flex;
flex-direction: column;
align-items: flex-start;
gap: 16.732px;
}
.links a {
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 16.732px;
font-style: normal;
font-weight: 600;
line-height: 150%; /* 25.098px */
}
p {
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 14.641px;
font-style: normal;
font-weight: 400;
line-height: 150%; /* 21.961px */
}
.credits-ctnr {
    gap: 20px;
}
.credits-divider{
    height: 1.046px;
align-self: stretch;
background: var(--Black, #000);
}
.credits-links {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    gap: 41px;
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 12px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
</style>