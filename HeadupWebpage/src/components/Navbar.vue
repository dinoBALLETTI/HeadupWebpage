<script>
</script>
<template>
    <div class="navframe">
        <div class="home_btn"><img src="../assets/medias/Logo.png"></div>
        <div class="burger_btn">
            <div class="solutions_btn ctnr">solutions</div>
            <div class="about_btn ctnr">Qui sommes nous?</div>
            <div class="blog_btn ctnr">Notre Blog</div>
            <div class="demo_btn ctnr">réserver une demo</div>
        </div>
    </div>
</template>

<style scoped>
.navframe{
    background-color: blueviolet;
    display: flex;
    height: 101px;
    padding: 0px 67.2px;
    justify-content: space-between;
    align-items: center;
    flex-shrink: 0;
    align-self: stretch; 
}

.burger_btn {
    display: flex;
    width: 751px;
    align-items: center;
    gap: 11.594px; 
}

.ctnr {
    font-family: Poppins;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: normal; 
}

</style>