<template>
    <div class="gains__intro">
        <h2>Avec Head Up, vos collaborateurs révèlent tout leur potentiel</h2>
        <h3>
            Notre programme de coaching mental inspiré par les techniques utilisées dans le sport de haut niveau offre à vos salariés les outils 
            et les stratégies nécessaires pour optimiser leur performance au travail.
        </h3>
    </div>
    
<div class="gains">
    
    <div class="gains__img">
        <img 
        src="../assets/medias/laptop.png" 
        style="
            width: 567.908px;
            height: 338.043px;
            transform: rotate(-0.373deg);"
            >
        </div>
        
    <div class="timeline-ctnr">
        <div class="timeline__content">

            <div class="timeline__items-ctnr">
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

            <div class="timeline__items-ctnr">
                <div class="item">
                    <span style="padding: 0px 12px 0px 12px"><img src="../assets/icons/clock.svg"></span>
                    <div class="divider"></div>
                </div>
                <div>
                    <span>
                        <a>20 minutes par semaine</a>
                        <p>Des formats courts et ludiques qui n’excèdent pas 20 minutes par semaine pour que vos collaborateurs se forment et progressent de façon continue sans impacter leur productivité.</p>
                    </span>
                </div>
            </div>

            <div class="timeline__items-ctnr">
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

            <div class="timeline__items-ctnr">
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
.gains {
    display: flex;
    flex-direction: column;
    padding: 35px;
    width: 100%;
}
.timeline__content {
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    gap: 16px;
}
.timeline__items-ctnr {
    display: flex;
    flex-direction: row;
    gap: 40px
}
.timeline__items-ctnr a {
    font-family: Poppins;
    font-style: normal;
    font-weight: 600;
    line-height: normal; 
    color: var(--Black, #000); 
}
.timeline__items-ctnr p {
    font-family: Open Sans;
    font-style: normal;
    font-weight: 400;
    line-height: normal; 
    text-align: justify;
    color: var(--Black, #000); 
}
.item {
    align-items: center;
    display: flex;
    flex-direction: column;
    gap: 16px;
    width: 60px;
}
.divider {
    background-color: black;
    height: 95%; 
    width: 4px;
}
.gains__img {
    align-items: center;
    direction: row;
    display: none; 
}
.gains__intro {
    padding: 25px;
    width: 100%;
}
@media screen and (min-width: 600px) {
    .gains {
        flex-direction: row;
        padding: 65px;
    }
    .gains__img {
        display:flex
    }
}
</style>