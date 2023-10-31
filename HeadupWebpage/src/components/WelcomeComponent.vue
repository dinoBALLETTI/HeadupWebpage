<script setup>
import Button from './shared/ButtonItem.vue'
</script>
<template>

<div class="header__ctnr">
    
    <div class="header__txt">
        <h1 class="header__txt--h1">Boostez les performances de vos salariés en développant leurs soft skills</h1>
        <h3 class="header__txt--h2">La solution de coaching inspirée de la préparation mentale des sportifs de haut de niveau pour développer les talents de votre entreprise. </h3>
    </div>
    <div class="header__btn">
        <Button :text="'Tester Head Up gratuitement'" link:="'/testpage'" />
    </div>

    <div class="header__img"><img src="../assets/medias/laptop.png"></div>
</div>

</template>

<style scoped>
/* *** SHARED PROPERTIES *** */
.header__ctnr {
    display: grid;
    grid-template-columns: 40% 60%;
    grid-template-rows: 1fr 1fr 1fr;
    height: 100vh;
    padding-left: 35px;
    width: 100%;
}
.header__txt {
    grid-column: 1 / 2;
    grid-row: 2;
}
.header__btn {
    grid-row: 3;
}
.header__img {
    align-items: center;
    background-image: url('../assets/medias/lady.png');
    background-position: bottom right;
    background-repeat: no-repeat;
    background-size: 75%;
    display: grid;
    grid-column: 2 / 3;
    grid-row: span 3;
}
.header__img img {
    max-width: 450px;  
}

/* *** MOBILE PROPERTIES *** */

@media screen and (max-width:900px) {
    .header__ctnr {
        display:flex;
        flex-direction: column;
        padding-right: 65px;
        padding-top: 100px;
    }
    .header__btn {
        display:none;
    }
}

/* *** DESKTOP PROPERTIES *** */

@media screen and (max-width:1100px) {
    .header__img {
        background-image: none;
    }
    .header__img img {
        max-width: 100%
    }
}
</style>
