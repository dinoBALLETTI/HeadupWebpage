<template>

    <div class="proposition__ctnr">
        <h2 class="text__1"><span class="big-text__1">Plus d’1 salarié sur 2</span> n’est pas satisfait de l’offre de formation de son entreprise.</h2>
        <h3 class="text__2">
            <p>Les formations sont souvent perçues comme étant peu collaboratives, trop descendantes et décorrélées des véritables problématiques des apprenants.</p>
            <p><span class="big-text__2">50% des collaborateurs</span> jugent que les formations proposées par l’entreprise ne couvrent pas les thématiques de développement personnel qu’ils recherchent, comme la RSE. Les soft skills, par exemple, ne semblent pas du tout être assez valorisées.</p>
            <p class="sources">*Baromètre de la formation 2023 réalisé par edFlex</p>
        </h3>
    </div>

</template>

<script setup>
</script>

<style scoped>
.proposition__ctnr {
    background: var(--violet-darker, #300080);
    color: #FFFFFF;
    display: grid;
    font-size: 24px;
    padding: 48px;
    width: 100%;
}
.text__1 {
    font-size: 16px
}
.big-text {
    font-size: 24px
}
.text__2{
    display: none;
}
.sources {
    color: var(--grises-white, #FFF);
    font-family: Open Sans;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    grid-row:2;
    justify-content: center;
    line-height: normal;
}

@media screen and (min-width: 600px) {
    .proposition__ctnr {
        align-items:center;
        column-gap: 83px;
        grid-template-columns: 1fr 1fr;
        padding: 100px 65px; 
    }

    .text__1 {
        color: var(--grises-white, #FFF);
        font-family: Poppins;
        font-size: 32px;
        font-style: normal;
        font-weight: 400;
        grid-column: 1;
        grid-row: 1;
        line-height: normal;
        width: 100%;
    }
    .big-text__1 {
        color: var(--grises-white, #FFF);
        font-family: Poppins;
        font-size: 48px;
        font-size: 48px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
    .text__2 {
        color: var(--grises-white, #FFF);
        display: block;
        display:flex;
        flex-direction: column;
        font-family: Open Sans;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        grid-column: 2;
        grid-row: 1;
        line-height: normal;
        width: 100%;
    }
    .big-text__2 {
        color: var(--grises-white, #FFF);
        font-family: Open Sans;
        font-size: 18px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
    }
    .sources {
        grid-column: 2;
    }
}
</style>