<template>
    <div class="button">
        <a :href="link">
            <div>{{ text }}</div>
        </a>
        <div class="arrow">
            <svg 
            width="10" 
            height="17" 
            viewBox="0 0 10 17" 
            fill="none" 
            xmlns="http://www.w3.org/2000/svg"
        >
        <g id="Group 1">
            <path 
                id="Vector" 
                fill-rule="evenodd" 
                clip-rule="evenodd" 
                d="M0.850147 1.17702C0.521678 1.50548 0.521678 2.03804 0.850147 2.36651L6.98418 8.50054L0.850147 14.6346C0.521678 14.963 0.521678 15.4956 0.850147 15.8241C1.17862 16.1525 1.71117 16.1525 2.03964 15.8241L8.76842 9.09529C9.09689 8.76682 9.09689 8.23426 8.76842 7.9058L2.03964 1.17702C1.71117 0.848547 1.17862 0.848547 0.850147 1.17702Z" 
                fill="white"
            />
        </g>
        </svg>
        </div>
    </div>
</template>


<script setup>
defineProps(['text', 'link'])
</script>

<style scoped>
.button {
    align-items: center;
    background: var(--violet-darker, #300080);
    border-radius: 25px;
    border: none;
    cursor: pointer;
    display: flex;
    font-family: Poppins;
    font-weight: 700;
    gap: 6.901px; 
    justify-content: center;
    padding: 10.352px 22.084px 10.352px 31.056px;
    text-decoration: none;
    transition: background 2s ease; 
    max-width: fit-content;
}

.button:hover {
    background: var(--gradient-violet-rose-dark, linear-gradient(180deg, #E4028D 0%, #6323CD 121.74%));
}

.button a {
    color: white;
    text-decoration: none;
}

.arrow {
    align-items: center; 
    display: flex;
    justify-content: center;
    width: 26.915px;
}
</style>
