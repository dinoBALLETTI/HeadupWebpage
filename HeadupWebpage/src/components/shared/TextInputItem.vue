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
    align-items: center;
    background: var(--White, #FFF);
    border-radius: 25px;
    border: 0.912px solid var(--grises-darkest, #20282C);
    display: flex;
    flex-direction: row;
    flex-shrink: 0;
    gap: 8px;
    justify-content: flex-end;
    padding: 1.5px;
    width: 100%;
}
input[type=text] {
    padding-left: 8px;
    width: 100%;
    background-color: none;
    outline-style: none;
}
</style>
