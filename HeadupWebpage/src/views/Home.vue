<script setup>
import Welcome from '../components/WelcomeComponent.vue'
import Partners from '../components/PartnersComponent.vue'
import Proposition from '../components/PropositionComponent.vue'
import Gains from '../components/GainsComponent.vue'
import Testimonial from '../components/TestimonialComponent.vue'
import Cta from '../components/CtaComponent.vue'
// import Blog from '../components/BlogComponent.vue'
// import FooterBlock from '../components/FooterBlockComponent.vue'
import Navbar from '../components/NavbarComponent.vue'

import BlogCardItem from '../components/shared/BlogCardItem.vue'

const posts = [
    {
    source: "https://media.glamour.com/photos/637ba22fdefafdff06cebb9e/16:9/w_1280,c_limit/653486498",
    theme: "Gestion du stress",
    title: "Un article sur la Lune",
    snippet: "le bon vieux lorem ipsum",
    time: "5 min",
    date: "Janvier 2023"
    },
    {
    source: null,    
    theme: "Gestion du stress",
    title: "Un article sur Mars",
    snippet: "le bon vieux lorem ipsum",
    time: "5 min",
    date: "Janvier 2023"
    },
    {
    source:"https://static.nationalgeographic.fr/files/styles/image_3200/public/thumb-1570438766.jpg?w=1600",    
    theme: "Gestion du stress",
    title: "Un article sur Mercure",
    snippet: "le bon vieux lorem ipsum",
    time: "5 min",
    date: "Janvier 2023"
    }
]
</script>

<template>
    <Navbar />
<div class="main-ctnr">

    <Welcome />
    <Partners />
    <Proposition />
    <Gains />
    <Testimonial />
    <Cta />
    <Blog />
    <FooterBlock />
    <div class="blogSection" v-for="(post, index) in posts" :key="index">
            
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
</template>

<style scoped>
.main_ctnr {
    width: 100%;
    height: 100%
}
</style>