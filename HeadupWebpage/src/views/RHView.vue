<script setup>
import { ref } from 'vue'
const email = ref('')
</script>
<template>
<div class="hr-contact__container">
    <div class="title__container">
        <div class="title">Parlez-en à mes RH !</div>
        <div class="intro">Laissez-nous l’email de votre responsable ou de votre RH ici ! 
            Merci pour votre aide et soyez assuré.e que nous garderons votre anonymat 🤫</div>
    </div>

    <div class="form__body">

        <span class="input-field">
                <label>Email professionnel<span class="asterisk">*</span></label>
                <input type="text" v-model="email">
        </span>
        <span class="input-field">
                <label>Nom de l'entreprise<span class="asterisk">*</span></label>
                <input type="text" v-model="email">
        </span>
    </div>
    
</div>
</template>
<style scoped>
.hr-contact__container {
    display:grid;
    gap: 5px;
    grid-template-columns: 1;
    grid-template-rows: 5;
    justify-items: center;
    padding: 115px 35px 40px;
    width: 100%;
}
input[type=text] {
    border-radius: 25px;
    border: 0.912px solid var(--grises-darkest, #20282C);
    padding: 12px 18px;
    width: 100%;
}</style>


