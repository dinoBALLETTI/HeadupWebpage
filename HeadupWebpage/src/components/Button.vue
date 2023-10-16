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
    margin: 35px;
    border: none;
    border-radius: 24.155px;
    background: var(--violet-darker, #300080);
    cursor: pointer
}
.button a div {
    color: white;
}
</style>