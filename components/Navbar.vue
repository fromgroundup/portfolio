<template>
    <div class="navbar">
        <div class="site-title">fromgroundup</div>
        <div><nuxt-link to="/">home</nuxt-link></div>
        <div><nuxt-link to="/portfolio">portfolio</nuxt-link></div>
        <div><nuxt-link to="/blog">blog</nuxt-link></div>
        <div><nuxt-link to="/contact">contact</nuxt-link></div>
        <div class="spacer"></div>
    </div>
</template>

<style scoped>
.navbar {
    display: flex;
    justify-content: space-evenly;
    font-family: 'Open Sans', sans-serif;
}

.spacer {
    flex-grow: 1;
}

a {
    text-decoration: transparent;
    color: black;
    margin: 2em;
    transition: text-decoration-color 1s;
}

a:hover {
    text-decoration: underline
}

.site-title {
    font-weight: 700;
    margin-left: 2em;
}
</style>