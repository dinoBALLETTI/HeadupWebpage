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
            <span class="time">{{ time }}</span>
            <span class="date">{{ date }}</span>
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
</style>