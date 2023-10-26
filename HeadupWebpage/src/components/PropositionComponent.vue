<template>
    <div class="proposition_ctnr">
        <h2 class="txt_ctnr1" style="font-family: Poppins font-weight:400;"><span style="font-size:24px">Plus d’1 salarié sur 2</span> n’est pas satisfait de l’offre de formation de son entreprise.</h2>
        <h3 class="txt_ctnr2">
            <p>Les formations sont souvent perçues comme étant peu collaboratives, trop descendantes et décorrélées des véritables problématiques des apprenants.</p>
            <p>50% des collaborateurs jugent que les formations proposées par l’entreprise ne couvrent pas les thématiques de développement personnel qu’ils recherchent, comme la RSE. Les soft skills, par exemple, ne semblent pas du tout être assez valorisées.</p>
        </h3>
        <h3 class="sources">
            <p>*Baromètre de la formation 2023 réalisé par edFlex</p>
        </h3>
    </div>

</template>

<script setup>
</script>

<style scoped>
.proposition_ctnr {
    display: flex;
    width: 100%;
    padding: 100px 65px;
    flex-direction: column;
    align-items: center;
    gap: 83.889px;
    background: var(--violet-darker, #300080);
    color: #FFFFFF;
    font-size: 24px
}
.txt_ctnr1 {
    width: 100%;
    font-size: 16px

}
.txt_ctnr2 {
    width: 100%;
    display: none;

}
@media screen and (min-width: 600px) {
    .proposition_ctnr {
        flex-direction: row;
        font-size: 48px
    }

.txt_ctnr1 {
    width: 100%;
}
.txt_ctnr2 {
    width: 100%;
    display: block;

}
}
</style>