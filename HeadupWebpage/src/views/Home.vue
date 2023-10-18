<script>
import Welcome from '../components/Welcome.vue'
import Partners from '../components/Partners.vue'
import Proposition from '../components/Proposition.vue'
import Gains from '../components/Gains.vue'
// import Testimonial from '../components/Testimonial.vue'
// import Cta from '../components/Cta.vue'
// import Blog from '../components/Blog.vue'
// import FooterBlock from '../components/FooterBlock.vue'
import Navbar from '../components/Navbar.vue'

export default {
    components: {
        Welcome,
        Partners,
        Proposition,
        Gains,
        // Testimonial,
        // Cta,
        // Blog,
        // FooterBlock,
        Navbar
    }
}
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