<script setup>
import { defineProps } from 'vue';

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
    <div class="card_ctnr">

        <div class="card_photo">
            <img class="topPic" :src="source">
            <div class="underlayer"></div>
        </div>

        <div class="theme">{{ theme }}</div>
        <div class="title">{{ title }}</div>
        <div class="snippet">{{ snippet }}</div>

        <div class="info">
            <div class="time">{{ time }}</div>
            <div class="date">{{ date }}</div>
        </div>

        <div class="link">
        <a :href="link">
            <div>Lire plus</div>
        </a>
        <div class="arrow">
            <svg 
            width="7.5" 
            height="15" 
            viewBox="0 0 10 17" 
            fill="none" 
            xmlns="http://www.w3.org/2000/svg"
        >
        <g id="Group 1">
            <path 
                id="Vector" 
                fill-rule="evenodd" 
                clip-rule="evenodd" 
                d="M0.850147 1.17702C0.521678 1.50548 0.521678 2.03804 0.850147 2.36651L6.98418 8.50054L0.850147 14.6346C0.521678 14.963 0.521678 15.4956 0.850147 15.8241C1.17862 16.1525 1.71117 16.1525 2.03964 15.8241L8.76842 9.09529C9.09689 8.76682 9.09689 8.23426 8.76842 7.9058L2.03964 1.17702C1.71117 0.848547 1.17862 0.848547 0.850147 1.17702Z" 
                fill="black"
            />
        </g>
        </svg>
        </div>
    </div>    </div>

</template>

<style scoped>
.card_ctnr {
    display: flex;
width: 447px;
height: 645.199px;
flex-direction: column;
align-items: flex-start;
gap: 25.138px;
flex-shrink: 0;
}
.topPic {
    width: 435.731px;
height: 314.229px;
flex-shrink: 0;
border-radius: 20px
}
.theme{
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
.title {
    color: var(--grises-darkest, var(--Grises-darkest, #20282C));
font-family: Poppins;
font-size: 28px;
font-style: normal;
font-weight: 600;
line-height: normal;
}
.info {
    display: flex;
    flex-direction: row;
    justify-content : space-between;
    width: 436px;
}
.snippet {
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
.time {
    color: var(--Black, #000);
font-family: Open Sans;
font-size: 14.664px;
font-style: normal;
font-weight: 600;
line-height: 150%;
}
.date {
    color: var(--Black, #000);
text-align: right;
font-family: Open Sans;
font-size: 14.664px;
font-style: normal;
font-weight: 600;
line-height: 150%;

}
.link {
    display: flex;
    flex-direction: row;
    color: #000;
    gap : 10px;

    font-family: Poppins;
font-size: 18px;
font-style: normal;
font-weight: 500;
line-height: normal;
text-decoration-line: underline;
}
</style>