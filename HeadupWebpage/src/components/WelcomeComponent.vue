<script setup>
import Button from './shared/ButtonItem.vue'
</script>
<template>
    <div class="spacer"></div>

<div class="header-ctnr">

        <div class="header__txt">
            <h1 class="header__txt--h1">Boostez les performances de vos collaborateurs en développant leurs soft skills</h1>
            <h3 class="header__txt--h2">La solution de coaching inspirée de la préparation mentale des sportifs de haut de niveau pour développer les talents de votre entreprise. </h3>
        </div>
        <div class="header__btn">
            <Button :text="'Tester Head Up gratuitement'" link:="'/testpage'" />
        </div>

        <div class="header__img"><img src="../assets/medias/laptop.png"></div>
</div>

</template>

<style scoped>
.header-ctnr {
    display: grid;
    grid-template-columns: 40% 60%;
    grid-template-rows: 1fr 1fr 1fr;
    width: 100%;
    padding-left: 65px;
    height: 100vh;
}
.header__txt {
    grid-column: 1 / 2;
    grid-row: 2;
}
.header__btn {
    grid-row: 3;
}
.header__img {
    display: grid;
    background-image: url('../assets/medias/lady.png');
    background-position: bottom right;
    background-repeat: no-repeat;
    background-size: 75%;
    grid-row: span 3;
    grid-column: 2 / 3;
    align-items: center;

}
.header__img img {
    max-width: 450px;  
}

@media screen and (max-width:1100px) {
.header__img {
    background-image: none;
}
.header__img img {
    max-width: 100%
}
}

@media screen and (max-width:900px) {
    .header-ctnr {
        display:flex;
        flex-direction: column;
        padding-top: 100px;
        padding-right: 65px
    }
    .header__btn {
        display:none;
    }


}
</style>
