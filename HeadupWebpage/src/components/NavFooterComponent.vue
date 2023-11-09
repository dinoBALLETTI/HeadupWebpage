<script setup>
import ButtonItem from './shared/ButtonItem.vue';
</script>

<template>
    <div class="footer">
        <div class="footer__btn"><ButtonItem :text="'/contact'" /></div>
    </div>
</template>
<style scoped>

.footer {
    display: grid;
    height: 100vh;
    padding: 0px 25px 25px 25px;
    position: fixed;
    width: 100%;
    justify-items: center;
}
.footer__btn {
    align-self: end;
    min-width: auto;
}

@media screen and (min-width: 900px) {
    .footer{
        display:none;
    }
}
</style>