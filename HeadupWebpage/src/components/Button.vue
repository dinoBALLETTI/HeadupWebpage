<template>
    <div class="button">
        <a :href="link">
            <div>{{ text }}</div>
        </a>
    </div>
</template>


<script setup>
defineProps(['text', 'link'])
</script>

<style scoped>
.button {
    padding: 0;
    border: none;
    border-radius: 24.155px;
    background: var(--violet-darker, #300080);
    text-decoration: none;
    cursor: pointer
}
</style>