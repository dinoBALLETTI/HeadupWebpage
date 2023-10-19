<script setup>
import Welcome from '../components/WelcomeComponent.vue'
import Partners from '../components/PartnersComponent.vue'
import Proposition from '../components/PropositionComponent.vue'
import Gains from '../components/GainsComponent.vue'
import Testimonial from '../components/TestimonialComponent.vue'
import Cta from '../components/CtaComponent.vue'
import Blog from '../components/BlogComponent.vue'
// import FooterBlock from '../components/FooterBlockComponent.vue'
import Navbar from '../components/NavbarComponent.vue'


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

</div>
</template>

<style scoped>
.main_ctnr {
    width: 100%;
    height: 100%
}
</style>