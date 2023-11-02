<template>

<div class="testimonial__ctnr">

    <!-- *** MOBILE GROUP *** -->
    <div class="quote__marks--start-mobile">
        <img  
        src="../assets/icons/quote-mobile.svg" 
        style="transform: rotate(179.224deg)"
        >
    </div>
    
    <div class="quote__text--mobile">J’essaie de changer mon discours intérieur et d’être plus positive depuis que j’ai fait le module et ça m’aide vraiment !</div>
    
    <div class="quote__marks--end-mobile">
        <img src="../assets/icons/quote-mobile.svg">
    </div>
    
    
    <!-- *** DESKTOP GROUP *** -->
    <div class="quote-container--desktop">

        
        <div class="quote__marks--start-desktop">
            <img  
            src="../assets/icons/quote-desktop.svg" 
            style="transform: rotate(179.224deg)"
            >
        </div>
        
        <div class="quote__text--desktop">J’essaie de changer mon discours intérieur et d’être plus positive depuis que j’ai fait le module et ça m’aide vraiment !</div>
        
        <div class="quote__marks--end-desktop">
            <img src="../assets/icons/quote-desktop.svg">
        </div>
        
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
    padding:35px;
    width: 100%;
    max-width: 1080px;
    margin: auto;
}
.quote__text--mobile, .quote__text--desktop {
    font-family: Open Sans;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    grid-column: 1;
    grid-row: 2;
    line-height: normal; 
    text-align: center;
}
.quote__marks--start-mobile {
    display: grid;
    grid-column: 1;
    grid-row: 1;
}
.quote__marks--end-mobile {
    display: grid;
    grid-column: 1;
    grid-row: 4;
    justify-self: end;
}
.quote-container--desktop {
    display:none;
    grid-column: 1;
    grid-row: 1;
    justify-content: space-between;
}
.quote__marks--end-desktop {
    justify-self: end;
}
.avatar__ctnr {
    display: flex;
    flex-direction: row;
    gap: 21px;
    grid-column: 1;
    grid-row:3;
    justify-content: center;
    padding-top: 16px;
}
.avatar__picture {   
    background: url(../assets/medias/avatarLucie.png);
    background-position: center;
    background-size: 100%;
    border-radius: 58.842px;
    height: 58.842px;
    width: 58.842px;
}
.avatar__name a {
    font-family: open Sans;
}

@media screen and (min-width: 600px) {
    .quote__text--desktop{
        font-size: 18px
    }
    .quote__marks--start-mobile, .quote__marks--end-mobile, .quote__text--mobile {
        display: none;
    }

    .testimonial__ctnr {
        padding: 100px 65px 100px 65px;
    }
    .quote-container--desktop {
        display: flex
    }
}
</style>