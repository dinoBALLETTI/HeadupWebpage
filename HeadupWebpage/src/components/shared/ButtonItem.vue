<script setup>
import Arrow from '@/assets/icons/arrow.svg'
defineProps(['text', 'link'])
</script>

<template>
    <div class="button">
        <a :href="link">
            <div>{{ text }}</div>
        </a>
        <div class="arrow">
            <img :src="Arrow">
         </div>
    </div>
</template>

<style scoped>
.button {
    align-items: center;
    background: var(--violet-darker, #300080);
    border-radius: 25px;
    border: none;
    cursor: pointer;
    display: flex;
    font-family: Poppins;
    font-weight: 700;
    gap: 6.901px; 
    justify-content: center;
    padding: 10.352px 22.084px 10.352px 31.056px;
    text-decoration: none;
    transition: background 2s ease; 
    max-width: fit-content;
}

.button:hover {
    background: var(--gradient-violet-rose-dark, linear-gradient(180deg, #E4028D 0%, #6323CD 121.74%));
}

.button a {
    color: white;
    text-decoration: none;
}

.arrow {
    align-items: center; 
    display: flex;
    justify-content: center;
    width: 26.915px;
}
</style>
