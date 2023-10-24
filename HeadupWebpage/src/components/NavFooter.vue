<script setup>
import ButtonItem from './shared/ButtonItem.vue';
</script>

<template>
    <div class="footer">
        <div class="footer__btn"><ButtonItem :text="'Réserver une démo'" /></div>
    </div>
</template>
<style scoped>

.footer {
    display: grid;
    height: 100vh;
    padding: 0px 25px 25px 25px;
    position: fixed;
    width: 100%;
}
.footer__btn {
    align-self: end;
    justify-items: center;
    min-width: auto;
}

@media screen and (min-width: 600px) {
    .footer{
        display:none;
    }
}
</style>