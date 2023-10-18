<template>
<h2>Avec Head Up, vos collaborateurs révèlent tout leur potentiel</h2>
<h3>
    Notre programme de coaching mental inspiré par les techniques utilisées dans le sport de haut niveau offre à vos salariés les outils 
    et les stratégies nécessaires pour optimiser leur performance au travail.
</h3>
    
<div class="gains_ctnr">
    
    <div style="
            display: flex; 
            direction: row;
            align-items: center">
        <img 
        src="../assets/medias/laptop.png" 
        style="
            width: 567.908px;
            height: 338.043px;
            transform: rotate(-0.373deg);"
            >
        </div>
        
    <div class="timeline_ctnr">
        <div class="timelineContent">

            <div class="timelineItem">
                <div class="item">
                    <span><img src="../assets/icons/diamond.svg"></span>
                    <div class="divider"></div>
                </div>
                <div>
                    <span>
                        <a>Un accès sans contrainte</a>
                        <p>Notre plateforme Head Up est disponible en accès illimité sur PC (et bientôt sur mobile) pour s’adapter aux contraintes et à l’emploi du temps de chacun.</p>
                    </span>
                </div>
            </div>

            <div class="timelineItem">
                <div class="item">
                    <span><img src="../assets/icons/clock.svg"></span>
                    <div class="divider"></div>
                </div>
                <div>
                    <span>
                        <a>20 minutes par semaine</a>
                        <p>Des formats courts et ludiques qui n’excèdent pas 20 minutes par semaine pour que vos collaborateurs se forment et progressent de façon continue sans impacter leur productivité.</p>
                    </span>
                </div>
            </div>

            <div class="timelineItem">
                <div class="item">
                    <span><img src="../assets/icons/weight.svg"></span>
                    <div class="divider"></div>
                </div>
                <div>
                    <span>
                        <a>Des outils concrets et faciles à mettre en pratique au quotidien</a>
                        <p>A chaque besoin, nous apportons une solution basée sur les techniques de la préparation mentale des sportifs de haut niveau : visualisation, discours interne, routines et répétition.</p>
                    </span>
                </div>
            </div>

            <div class="timelineItem">
                <div class="item">
                    <span><img src="../assets/icons/contactBubble.svg"></span>
                    <div class="divider"></div>
                </div>
                <div>
                    <span>
                        <a>Un accès sans contrainte</a>
                        <p>Nous vous accompagnons de la mise en place de la plateforme au suivi de la progression de vos équipes. Nous sommes là aussi pour engager plus largement votre entreprise sur les développements des compétences comportementales.</p>
                    </span>
                </div>
            </div>

        </div>
    </div>
</div>
</template>

<style scoped>
.gains_ctnr {
    display: flex;
    flex-direction: row;
}
.timelineContent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 16px;
    flex: 1 0 0; 
}
.timelineItem {
    display: flex;
    flex-direction: row;
    gap: 40px
}
.timelineItem a {
    font-family: Poppins;
    font-style: normal;
    font-weight: 600;
    line-height: normal; 
}
.timelineItem p {
    font-family: Open Sans;
    font-style: normal;
    font-weight: 400;
    line-height: normal; 
}
.item {
    width: 60px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px
}
.divider {
    width: 4px;
    height: 100px; 
    background-color: black;
}
</style>