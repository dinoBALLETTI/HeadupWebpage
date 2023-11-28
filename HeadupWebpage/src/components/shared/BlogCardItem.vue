<script setup>
import { defineProps } from 'vue';
import Arrow from '@/assets/icons/arrow-dark.svg'

const props = defineProps({
    source: {
        type: String,
        default: ''
    },    
    theme: String,
    title: String,
    snippet: String,
    time: String,
    date: String,
    link: String,
});
</script>

<template>
<div class="card__container">

    <div class="card__photo">
        <img class="card__photo--top-pic" :src="source">
        <div class="card__photo--underlayer"></div>
    </div>

    <div class="card__theme">{{ theme }}</div>
    <div class="card__title">{{ title }}</div>
    <div class="card__snippet">{{ snippet }}</div>

    <div class="info__container">
        <div class="info__time">{{ time }}</div>
        <div class="info__date">{{ date }}</div>
    </div>

    <div class="link">
        <a :href="link">
            <div>Lire plus</div>
        </a>
        <div class="arrow">
            <img :src="Arrow" fill="black">
        </div>
    </div>    
</div>
</template>

<style scoped>
.card__container {
    width: 100%;
    display: flex;
flex-direction: column;
align-items: flex-start;
gap: 12px;
flex-shrink: 0;
}
.card__photo {
    display: grid;
    grid-template-columns: 1;
    grid-template-rows: 1;
}
.card__photo--top-pic {
width: 100%;
border-radius: 20px;
grid-column: 1;
grid-row: 1;
z-index: 2;
}
.card__photo--underlayer {
width: 100%;
transform: rotate(2deg);
flex-shrink: 0;
border-radius: 20px;
background: var(--vert-primaire-neutral, #6DDDD0);
z-index: 1;
grid-column: 1;
grid-row: 1;
}
.card__theme{
    display: flex;
height: 30px;
padding: 10px 20px;
justify-content: center;
align-items: center;
gap: 10px;
border-radius: 30px;
background: var(--grises-darkest, #20282C);
color: #F0F3F4;
font-family: Open Sans;
font-size: 12px;
font-style: normal;
font-weight: 400;
line-height: normal;
letter-spacing: 0.72px;
text-transform: uppercase; 
}
.card__title {
    color: var(--grises-darkest, var(--Grises-darkest, #20282C));
font-family: Poppins;
font-size: 28px;
font-style: normal;
font-weight: 600;
line-height: normal;
}
.info__container {
    display: flex;
    flex-direction: row;
    justify-content : space-between;
    width: 100%;
}
.card__snippet {
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
.info__time {
    color: var(--Black, #000);
font-family: Roboto;
font-size: 10.5px;
font-style: normal;
font-weight: 600;
line-height: 150%; /* 15.633px */}
.info__date {
    color: var(--Black, #000);
text-align: right;
font-family: Roboto;
font-size: 10.5px;
font-style: normal;
font-weight: 600;
line-height: 150%;
}
.link {
    display: flex;
    flex-direction: row;
    color: #000;
    gap : 10px;

    color: #000;
font-family: Poppins;
font-size: 12.793px;
font-style: normal;
font-weight: 500;
line-height: normal;
text-decoration-line: underline;
cursor: pointer;
}

@media screen and (min-width:600px) {
    
}

</style>
