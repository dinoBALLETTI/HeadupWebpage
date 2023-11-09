<script setup>
import ButtonItem from '../components/shared/ButtonItem.vue';
</script>
<template>


<div class="form__container">
    <div class="form__title">Demander une démo</div>
    <div class="form__description">Avec Head Up, vous pourrez mettre en place une culture apprenante au service de la performance de votre entreprise. </div>
    <div class="form__body"></div>
    <div class="button"><ButtonItem :text="'Contactez-nous'"/></div>
    <div class="form__footer">Vous êtes un particulier et apprendre des techniques pour développer votre potentiel vous intéresse ? Notre service n’est pas disponible pour le grand public mais vous pouvez nous aider à contacter votre RH !  👋​</div>
</div>



</template>
<style scoped>
.form__container {
    display:grid;
    grid-template-columns: 1;
    grid-template-rows: 5;
    padding: 115px 80px 65px;
    width: 100%;
    justify-items: center;
    gap: 5px
 
}
.form__title {
    color: #000;
    font-family: Poppins;
    font-size: 32px;
    font-style: normal;
    font-weight: 800;
    grid-column: 1;
    grid-row: 1;
    line-height: normal;
    text-align: center;
}
.form__description {
    grid-column: 1;
    grid-row: 2;
    width: minmax(100%, 680px);
    color: #000;
text-align: center;
display: flex;
width: 388px;
padding: 0px 35px;
flex-direction: column;
justify-content: center;
align-items: flex-start;
gap: 8px;

/* Mobile - Corps */
font-family: Open Sans;
font-size: 16px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
.form__body {
    grid-column: 1;
    grid-row: 3;
    max-width: 680px;

}
.button {
    grid-column: 1;
    grid-row: 4;
}
.form__footer {
    grid-column: 1;
    grid-row: 5;
    max-width: 680px;

}

</style>