<script>
</script>
<template>
    <div class="news" v-if="newsStatus">
        <div class="newsText">Message nouveauté avec lien de redirection</div>
        <div class="newsBtn" @click="toggleNews">
            <svg 
                width="32" 
                height="32" 
                viewBox="0 0 32 32" 
                fill="none" 
                xmlns="http://www.w3.org/2000/svg"
            >
            <path 
                d="M22.8354 22.3644L22.3639 22.8358C22.1036 23.0961 21.6815 23.0961 21.4211 22.8358L16 17.4146L10.5788 22.8357C10.3185 23.0961 9.89638 23.0961 9.63603 22.8357L9.16462 22.3643C8.90427 22.104 8.90427 21.6819 9.16462 21.4215L14.5858 16.0004L9.16462 10.5792C8.90427 10.3189 8.90427 9.89675 9.16462 9.6364L9.63602 9.165C9.89637 8.90465 10.3185 8.90465 10.5788 9.165L16 14.5862L21.4211 9.16499C21.6815 8.90464 22.1036 8.90464 22.3639 9.16499L22.8354 9.63639C23.0957 9.89674 23.0957 10.3189 22.8354 10.5792L17.4142 16.0004L22.8354 21.4215C23.0957 21.6819 23.0957 22.104 22.8354 22.3644Z" 
                fill="white"
            />
            </svg>
        </div>
    </div>

    <div class="navframe">
        <div class="home_btn"><img src="../assets/medias/Logo.png"></div>
        <div class="burger_btn">
            <div class="solutions_btn ctnr">solutions</div>
            <div class="about_btn ctnr">Qui sommes nous?</div>
            <div class="blog_btn ctnr">Notre Blog</div>
            <div class="demo_btn ctnr">
                <Button :text="'Réserver une démo'" :link="'your-demo-link'"/>
            </div>
        </div>
    </div>
</template>

<script setup>
import Button from './Button.vue'
import { ref } from 'vue'

const newsStatus = ref(true);
const toggleNews = () => {
    newsStatus.value = false
}

</script>

<style scoped>
.news {
    align-items: center;
    align-self: stretch;
    background: var(--orange-dark, #CB6E01);
    color: var(--grises-white, #FFF); 
    display: flex;
    flex-direction: row-reverse;
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    gap: 16px;
    line-height: normal; 
    padding: 8px 65px;
}
.navframe{
    /* background-color: blueviolet; */
    align-items: center;
    align-self: stretch; 
    display: flex;
    flex-shrink: 0;
    height: 101px;
    justify-content: space-between;
    padding: 0px 65px;
    gap: 40px
}
.home_btn {
    align-items: center;
    display: flex;
    gap: 40px; 
    padding: 5px 0px;
    width: 853px;
}
.burger_btn {
    align-items: center;
    display: flex;
    gap: 11.594px; 
    width: 751px;
}

.ctnr {
    font-family: Poppins;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: normal; 
    white-space: nowrap;
}

</style>