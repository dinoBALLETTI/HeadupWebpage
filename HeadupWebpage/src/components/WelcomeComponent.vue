<template>
<div class="header_ctnr">
        <div class="header_txt">
            <h1 class="header_txt1">Boostez les performances de vos collaborateurs en développant leurs soft skills</h1>
            <h3 class="header_txt2">La solution de coaching inspirée de la préparation mentale des sportifs de haut de niveau pour développer les talents de votre entreprise. </h3>
            <div class="header_btn">
                <Button :text="'Tester Head Up gratuitement'" link:="'/testpage'" />
            </div>
        </div>
        <div class="header_img">
        </div>
    </div>
</template>

<script setup>
import Button from './shared/ButtonItem.vue'
</script>

<style scoped>

.header_ctnr {
    background-color: #F3FCFB;
    display: flex;
    flex-direction: row;
    align-items: center;
}
.header_txt {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 25px;
    width: 593px;
    width: 592px;
    padding-left: 65px;
    padding-right: 30px
}
.header_txt1 {
/* font-family: Poppins;
font-weight: 800; */
 display: flex;

}

.header_txt2 {
    display: flex;
    text-align: justify;
    /* font-family: Open Sans;
font-weight: 400; */
}

.header_btn {
    display: flex;
}
.header_img{
    width: 800px;
height: 700px; 
flex-shrink: 0; 
background-position-x: center;
background-position-y: bottom;
background-image: url('../assets/medias/headerPictures.png');

}

</style>