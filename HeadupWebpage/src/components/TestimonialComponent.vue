<template>

<div class="testimonial__ctnr">

    <div class="quote__marks--start">
        <img  
        src="../assets/icons/quote.svg" 
        style="transform: rotate(179.224deg)"
        >
    </div>

    <div class="quote__text">J’essaie de changer mon discours intérieur et d’être plus positive depuis que j’ai fait le module et ça m’aide vraiment !</div>
    
    <div class="quote__marks--end">
        <img src="../assets/icons/quote.svg">
    </div>

    <div class="avatar__ctnr">
        <div class="avatar__picture"></div>

        <div class="avatar__name"
            style="
            display: flex;
            flex-direction: column;
            "
            >
            <a style="
                color: var(--Black, #000);
                font-style: normal;
                font-weight: 600; 
                "
            >Lucie</a>
            
            <a>Cheffe de produit</a>
        </div>
    </div>
 
</div>

</template>

<style scoped>
.testimonial__ctnr {

display:grid;
grid-template-columns: 1;
grid-template-rows: 4;
row-gap: 16px;
padding:35px;
width: 100%
}
.quote__text {
    font-family: Open Sans;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: normal; 
    grid-row: 2;
    grid-column: 1;
    text-align: center;
}
.quote__marks--start {
    display: block;
    width: 60px;
height: 60px; 
grid-row: 1;
grid-column: 1;

}
.quote__marks--end {
display: block;
    width: 60px;
height: 60px; 
grid-row: 4;
grid-column: 1;
}

.avatar__ctnr {
    display: flex;
    flex-direction: row;
    gap: 21px;
    grid-row:3;
    grid-column: 1;
    justify-content: center;

}
.avatar__picture {   

    width: 58.842px;
    height: 58.842px;
    border-radius: 58.842px;
    background: url(../assets/medias/avatarLucie.png);
    background-position: center;
    background-size: 100%;
}
.avatar__name a {
    font-family: open Sans;
}

@media screen and (min-width: 600px) {
    .quote__marks--start {
        width: 100px;
        height: 100px; 
    }
    .quote__marks--end {
        width: 100px;
        height: 100px; 
    }
    .quote__text{
        font-size: 18px
    }
}
</style>