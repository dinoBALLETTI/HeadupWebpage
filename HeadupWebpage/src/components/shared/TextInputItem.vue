<script setup>
import ButtonItem from './ButtonItem.vue';
defineProps('inputText')
</script>

<template>
    <div class="input-field__container">
        <input type="text" :placeholder="inputText">
        <ButtonItem :text="`M'inscrire`" />
    </div>
</template>

<style scoped>
.input-field__container {
    flex-direction: row;
    width: 100%;
    display: flex;
    padding: 1.5px;
    align-items: center;
    justify-content: flex-end;
    gap: 8px;
    flex-shrink: 0;
    border-radius: 25px;
    border: 0.912px solid var(--grises-darkest, #20282C);
    background: var(--White, #FFF);
}
input[type=text] {
    padding-left: 8px;
    width: 100%;
    background-color: none;
    outline: none !important;
}
</style>
