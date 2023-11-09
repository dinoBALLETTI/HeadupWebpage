<script setup>
import { RouterView } from 'vue-router'
import NavHeaderComponent from './components/NavHeaderComponent.vue';
import NavFooterComponent from './components/NavFooterComponent.vue';
import FooterBlockComponent from './components/FooterBlockComponent.vue';
</script>

<template>
    <NavHeaderComponent />
    <NavFooterComponent />
    <FooterBlockComponent />
    
    <RouterView />
</template>
