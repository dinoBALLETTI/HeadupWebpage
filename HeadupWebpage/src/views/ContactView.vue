<script setup>
// import { ref } from 'vue';
import ButtonItem from '../components/shared/ButtonItem.vue';

</script>
<template>

<div class="form__container">

    <div class="form__title">Demander une démo</div>
    <div class="form__description">Avec Head Up, vous pourrez mettre en place une culture apprenante au service de la performance de votre entreprise. </div>
    
    <div class="form__body">
        <form>
            <div class="names__container">
                <span class="input-field--last-name">
                    <label>Nom<span class="asterisk">*</span></label>
                    <input type="text" v-model="lastName">
                </span>
                <span class="input-field--first-name">
                    <label>Prénom<span class="asterisk">*</span></label>
                    <input type="text" v-model="firstName">
                </span>
            </div>
            <span class="input-field">
                <label>Email professionnel<span class="asterisk">*</span></label>
                <input type="text" v-model="firstName">
            </span>
            <span class="input-field">
                <label>Numéro de téléphone<span class="asterisk">*</span></label>
                <input type="text" v-model="firstName">
            </span>
            <span class="input-field">
                <label>Nom de l'entreprise<span class="asterisk">*</span></label>
                <input type="text" v-model="firstName">
            </span>
            <span class="input-field">
                <label>Nombre de salariés<span class="asterisk">*</span></label>
                <input type="text" v-model="firstName">
            </span>
        </form>
    </div>

    <div class="button"><ButtonItem :text="'Contactez-nous'"/></div>

    <div class="form__footer">Vous êtes un particulier et apprendre des techniques pour développer votre potentiel vous intéresse ? Notre service n’est pas disponible pour le grand public mais vous pouvez nous aider
        <a class="rh" href="/hr-contact">à contacter votre RH !  </a>👋​
    </div>

</div>

</template>
<style scoped>
.form__container {
    display:grid;
    gap: 5px;
    grid-template-columns: 1;
    grid-template-rows: 5;
    justify-items: center;
    padding: 115px 35px 40px;
    width: 100%;
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
    padding-bottom: 12px;
    text-align: center;
    width:100%;
}
.form__description {
    align-items: flex-start;
    color: #000;
    display: flex;
    flex-direction: column;
    font-family: Open Sans;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    gap: 8px;
    grid-column: 1;
    grid-row: 2;
    justify-content: center;
    line-height: normal;
    max-width: 680px;
    padding: 0px 35px;
    text-align: center;
    width:100%;
}
.form__body {
    align-items: center;
    display: flex;
    flex-direction: column;
    gap: 36px;
    grid-column: 1;
    grid-row: 3;
    max-width: 680px;
    padding: 48px 35px;
}
.names__container {
    display: flex;
    flex-direction: column;
}
input[type=text] {
    border-radius: 25px;
    border: 0.912px solid var(--grises-darkest, #20282C);
    padding: 12px 18px;
    width: 100%;
}
label {
    color: var(--grises-darkest, #20282C);
    font-family: Poppins;
    font-size: 16px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    padding: 0px 10px; 
}
.asterisk {
    color: var(--rouge-dark, #CF2300);
}
.button {
    grid-column: 1;
    grid-row: 4;
}
.form__footer {
    color: #000;
    grid-column: 1;
    grid-row: 5;
    max-width: 680px;
    font-family: Open Sans;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding: 36px
}
.rh {
    color: #000;
    cursor: pointer;
    font-family: Open Sans;
    font-size: 16px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    text-decoration-line: underline;
}
@media screen and (min-width: 600px) {
    .names__container {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1;
        gap:8px;
    }
    .form__title {
        padding-bottom: 25px;
    }
}
</style>