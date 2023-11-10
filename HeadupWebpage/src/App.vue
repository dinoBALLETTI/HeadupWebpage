<script setup>
import { RouterView } from 'vue-router'
import NavHeaderComponent from './components/NavHeaderComponent.vue';
// import NavFooterComponent from './components/NavFooterComponent.vue';
import FooterBlockComponent from './components/FooterBlockComponent.vue';
</script>

<template>
    <NavHeaderComponent />
    <!-- <NavFooterComponent /> -->
    <!-- *** NavFooter have a different display priority, to use DevTools mor comfortably, comment the component and its import -->
    
    <RouterView />
    
    <FooterBlockComponent />
</template>
