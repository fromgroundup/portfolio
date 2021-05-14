<template>
    <div class="listing">
        <nuxt-link :to="'/post/' + preview.slug">
            <div class="heading">{{preview.title}}</div>
            <div class="heading">{{preview.subtitle}}</div>
            <div class="content">{{preview.updatedAt}}</div>
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