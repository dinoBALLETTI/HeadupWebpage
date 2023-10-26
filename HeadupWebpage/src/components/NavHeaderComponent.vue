<script setup>
import { ref } from 'vue';
import CrossIcon from '@/assets/icons/cross.svg';
import ButtonItem from './shared/ButtonItem.vue';
import Burger from '@/assets/icons/burger.svg'

const newsStatus = ref(true);
const toggleNews = () => {
    newsStatus.value = false
};

const menuStatus = ref(false);
const toggleMenu = () => {
    menuStatus.value = !menuStatus.value;
};
</script>
<template>
<div class="nav-ctnr">
    <div class="news" v-if="newsStatus">
        <div class="news-button" @click="toggleNews" style="cursor: pointer">
            <img :src="CrossIcon">
        </div>
        
        <div class="news-text">Message nouveauté avec lien de redirection</div>
    </div>
    
<!-- *** DESKTOP GROUP *** -->
    <div class="nav--desktop" id="myNav">
        <div class="nav__logo">
            <img src="../assets/medias/Logo.png">
        </div>
        <div class="links--desktop">

            <a href="/solutions">Notre Solution</a>
            <a href="/about">Qui sommes nous ?</a>
            <a href="/blog">Notre Blog</a>
            
            <div class="nav__demo-button">
            <ButtonItem :text="'Réserver une démo'" :link="'your-demo-link'" />
        </div>
    </div>

    </div>

<!-- *** MOBILE GROUP *** -->
    <div class="nav--mobile">
        <div class="nav__logo--mobile">
            <img src="../assets/medias/Logo.png">
        </div>
        <div class="icon" @click="toggleMenu">
            <img :src="Burger">
        </div>
    </div>
    <div class="links--mobile" v-if="menuStatus">
        <a href="/solutions">Notre Solution</a>
        <a href="/about">Qui sommes nous ?</a>
        <a href="/blog">Notre Blog</a>

    </div>
</div>
</template>

<style scoped>

.nav-ctnr {
position: fixed;
width: 100%;
height: auto;
z-index: 5;
padding: 0px 65px 0px 65px ;

}
.news {
    align-items: center;
    background: var(--orange-dark, #CB6E01);
    color: var(--grises-white, #FFF); 
    display: none;
    flex-direction: row-reverse;
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    gap: 16px;
    justify-content: space-around;
    line-height: normal; 
    padding: 8px ;
}
.nav--desktop {
    display: none;
    height: 100px;
    background-color: #FFF;
}
.nav--mobile{
    display: grid;
    grid-template-columns: 85% 15%;
    background: #FFF;
    align-content: center;
}
.links--mobile {
    display: grid;
}
.links--mobile a {
    border-bottom: 1px solid var(--grises-light, #A6B7BF);
    background: #FFF;
    padding: 8px;
    font-family: Open Sans;
    font-weight: 400;
    text-decoration: none;
    color:black
}
.icon   {
    display: grid;
    margin: auto;
    cursor: pointer;
}

@media screen and (min-width: 1100px) {
    .nav--desktop {
        display: grid;
        grid-template-columns: 20% 80%;
        align-content: center;
    }
    .nav--mobile {
        display: none;
    }
    .nav__logo {
    grid-column: 1;
    }
    .links--desktop {
        align-items: center;
        display: flex ;
        flex-direction: row;
        font-family: Poppins;
        font-weight: 700;
        gap: 40px;
        grid-column: 2;
        grid-row: 1;
        justify-content: end;
        background-color: #FFF;
        white-space: nowrap;
    }
    .links--desktop a {
        text-decoration: none;
        color: black;
    }

}

</style>