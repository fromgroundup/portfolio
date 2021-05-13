<template>
    <div class="navbar">
        <div><nuxt-link to="/">Home</nuxt-link></div>
        <div><nuxt-link to="/portfolio">Portfolio</nuxt-link></div>
        <div><nuxt-link to="/blog">Blog</nuxt-link></div>
        <div><nuxt-link to="/contact">Contact</nuxt-link></div>
    </div>
</template>

<style>
.navbar {
    display: flex;
    justify-content: space-evenly;
}
</style>