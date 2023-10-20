<script setup>
import { ref } from 'vue';
import CrossIcon from '@/assets/icons/cross.svg';
import ButtonItem from './shared/ButtonItem.vue';
import Burger from '@/assets/icons/burger.svg'

const newsStatus = ref(true);
const toggleNews = () => {
    newsStatus.value = false
}

const toggleBurger = () => {
  var x = document.getElementById("myNav");
  if (x.className === "nav") {
    x.className += " responsive";
  } else {
    x.className = "nav";
  }
} 
</script>
<template>
    <div class="news" v-if="newsStatus">
        <div class="news-button" @click="toggleNews" style="cursor: pointer">
            <img :src="CrossIcon">
        </div>

        <div class="news-text">Message nouveauté avec lien de redirection</div>
    </div>

    <div class="nav" id="myNav">
        <!-- *** Ajouter les liens dans href="" pour chaque <a></a>*** -->
        <div class="nav__logo">
            <img src="../assets/medias/Logo.png">
        </div>
        <a>Notre Solution</a>
        <a>Qui sommes nous?</a>
        <a>Notre Blog</a>
        <div class="nav__demo-button">
            <ButtonItem :text="'Réserver une démo'" :link="'your-demo-link'" />
        </div>
        <a href="javascript:void(0);" class="icon" @click="toggleBurger">
            <img :src="Burger">
        </a>
    </div>
</template>



<style scoped>
.news {
    align-items: center;
    background: var(--orange-dark, #CB6E01);
    color: var(--grises-white, #FFF); 
    display: flex;
    flex-direction: row-reverse;
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    gap: 16px;
    justify-content: space-between;
    line-height: normal; 
    padding: 8px 65px;
}
.nav {
    align-items: center;
    align-self: stretch;
    background: var(--vert-primaire-lightest, #F3FCFB);
    display: flex;
    flex-shrink: 0;
    height: 100px;
    justify-content: space-between;
    padding: 0px 67px;
}
.nav .icon {
    display: none;
}

@media screen and (max-width: 600px) {
    .nav {
        padding: 35px;
    }
    .nav a {display: none;}
    .nav__demo-button {display: none;}
    .nav a.icon {
        float: right;
        display: block;
    }
}

@media screen and (max-width: 600px) {
  .nav.responsive {position: relative;}
  .nav.responsive a.icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .nav.responsive a {
    display: block;
    float: none;
    text-align: left;
  }
}
</style>