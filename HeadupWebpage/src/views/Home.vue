<script>
import Welcome from './Welcome.vue'
export default {
    components: {
        Welcome,
    }
}
</script>

<template>
<div class="main-ctnr">

    <Welcome />

    <div class="partners_ctnr">
        <h2>parteniares</h2>
        <div class="partners_carousel">le carousel</div>
    </div>

    <div class="gains_ctnr">
        <h2>benefices</h2>
        <h3>lrem</h3>

        <div style="display: flex; direction: row;">
            <img src="../assets/images/laptop.png">
            <div class="gains_divider">petites icones</div>
            <div class="gains_txt">
                <p>kjsdfds</p>
                <p>kjsdfds</p>
                <p>kjsdfds</p>
                <p>kjsdfds</p>
            </div>
        </div>
    </div>

    <div class="testimonial_ctnr">
        <h3>lsdkfld</h3>
        <div class="quote_ctnr" style="display: flex; flex-direction: row">
            <div class="quote_img">image de lucie</div>
            <div class="quote_txt">
                <p>lucie</p>
                <p>lkjsdfdslkjf</p>
            </div>
        </div>
    </div>

    <div class="cta_ctnr">
        <h2>le cta</h2>
        <h3>le blablalkdsjflkj</h3>
        <div class="cta_btn"></div>
    </div>
    
    <div class="blog_ctnr">
        <h2>ressoruces utiles</h2>
        <h3>sdjfljdsfl</h3>
        <div class="blog_components">
            <!-- v-for article in articles -->
        </div>
    </div>

    <div class="footer_ctnr">
        <div class="newsletter_ctnr">
            <!-- <img src=" ????">logo headup -->
            <h3>ne ratez pas nos artciles</h3>
            <input type="text">
            <div class="newsletter_btn"></div>
        </div>

        <div class="solutions_ctnr">
            <h3>link 1</h3>
            <h3>link 2</h3>
        </div>

        <div class="about_ctnr">
            <h3>qui?</h3>
            <h3>blog</h3>
        </div>

        <div class="networks_ctnr">
            <!-- img + link
            img + link -->
        </div>
    </div>

</div>

</template>

<style scoped>
.main_ctrn {
    padding: 0px 85px 0px 65px; }
</style>