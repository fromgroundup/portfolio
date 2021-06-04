<template>
    <div class="listing">
        <nuxt-link :to="'/post/' + preview.slug">
            <div class="open-sans">{{preview.title}}</div>
            <div class="open-sans">{{preview.subtitle}}</div>
            <div class="montserrat">{{preview.updatedAt}}</div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    props: ['preview']
}
</script>

<style scoped>
.listing {
    /* Flexbox rules */
    display: flex;
    flex-direction: column;
    /* General spacing rules */
    margin: 2em;
}
</style>