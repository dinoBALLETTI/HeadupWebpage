<script setup>
import BlogCardItem from '../components/shared/BlogCardItem.vue'
import ButtonItem from './shared/ButtonItem.vue';

const posts = [
    {
    source: "https://media.glamour.com/photos/637ba22fdefafdff06cebb9e/16:9/w_1280,c_limit/653486498",
    theme: "Gestion du stress",
    title: "Un article sur la Lune",
    snippet: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.",
    time: "5 min",
    date: "Janvier 2023"
    },
    // {
    // source: null,    
    // theme: "Gestion du stress",
    // title: "Un article sur Mars",
    // snippet: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.",
    // time: "5 min",
    // date: "Janvier 2023"
    // },
    // {
    // source:"https://static.nationalgeographic.fr/files/styles/image_3200/public/thumb-1570438766.jpg?w=1600",    
    // theme: "Gestion du stress",
    // title: "Un article sur Mercure",
    // snippet: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros.",
    // time: "5 min",
    // date: "Janvier 2023"
    // }
]
</script>
<template>

    <div class="main__container"> 

        <div class="text__container">
            <h2>Nos ressources utiles</h2>
            <h3>Des conseils sur les thématiques de la préparation mentale, du coaching et de l’accompagnement des RHs.</h3>
        </div>
       
        <div class="blog__container">

            <div class="blog--section" v-for="(post, index) in posts" :key="index">
                
                <BlogCardItem 
                :source="post.source"
                :title="post.title"
                :snippet="post.snippet"
                :time="post.time"
                :date="post.date"
                :theme="post.theme"
                />
            </div>
        </div>

        <ButtonItem :text="'Voir les articles'" :link="'tbd'" />

    </div>
 
</template>

<style scoped>

.main__container {
    display: flex;
    width: 100%;
    padding: 0px 35px;
    flex-direction: column;
    align-items: center;
    gap: 36px;
}
.text__container {
    display:flex;
    flex-direction: column;
    align-items: center;
}
.text__container h2 {
color: var(--grises-darkest, var(--Grises-darkest, #20282C));
text-align: center;
font-family: Poppins;
font-size: 24px;
font-style: normal;
font-weight: 700;
line-height: normal;
}
.text__container h3 {
    color: var(--Black, #000);
text-align: center;

font-family: Open Sans;
font-size: 16px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
.blog__container {
    width: 100%;
}
.blog--section {
    width: 100%;
}
</style>