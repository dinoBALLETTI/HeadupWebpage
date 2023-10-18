<template>

<div class="quote_ctnr">

    <div class="quote">
    <img src="../assets/icons/quote.svg" 
        style="
            width: 100px;
            height: 100px;
            transform: rotate(179.224deg)
        "
    >
    <div class="quote_txt">J’essaie de changer mon discours intérieur et d’être plus positive depuis que j’ai fait le module et ça m’aide vraiment !</div>
    <img src="../assets/icons/quote.svg" 
        style="
            width: 100px;
            height: 100px;
        "
    >
    </div>

    <div class="avatar_ctnr">
        <div class="witnessAvatar"></div>
        <div class="avatarName"
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
.quote_ctnr {

    display: flex;
    padding: 100px 65px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 50.436px; 
}
.quote_txt {
    font-family: Open Sans;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: normal; 
}
.quote {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-evenly;
}
.avatar_ctnr {
    display: flex;
    flex-direction: row;
    gap: 21px
}
.witnessAvatar {
    width: 58.842px;
    height: 58.842px;
    border-radius: 58.842px;
    background: url(../assets/medias/avatarLucie.png);
    background-position: center;
    background-size: 100%;
}
.avatarName a {
    font-family: open Sans;
}
</style>