<template>
    <div class="skill-listing">
        <nuxt-link :to="'/skill/' + skill.slug">
            <div class="heading">{{skill.name}}</div>
            <div class="content">{{skill.summary}}</div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    props: ['skill']
}
</script>

<style scoped>
.skill-listing {
    /* Flexbox rules */
    display: flex;
    flex-direction: column;
    /* General spacing rules */
    margin: 2em;
}
</style>