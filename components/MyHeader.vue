<script setup lang="ts">
const navItems = [
    {
        text: "Projects",
        link: "/",
    },
    {
        text: "About",
        link: "/",
    },
    {
        text: "Experience",
        link: "/",
    },
    {
        text: "Contact",
        link: "/",
    },
];
</script>
<template>
    <header class="py-4 flex items-center justify-center">
        <nav class="flex items-center bg-[#3b3b3b] rounded-lg py-4">
            <NuxtLink
                v-for="(item, index) in navItems"
                :to="item.link"
                :key="index"
                class="hover:text-green-300 mx-6 text-white text-lg font-bold"
                >{{ item.text }}</NuxtLink
            >
        </nav>
    </header>
</template>

