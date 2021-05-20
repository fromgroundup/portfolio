<template>
    <div class="project-listing">
        <nuxt-link :to="'/project/' + project.slug">
            <div class="heading">{{project.name}}</div>
            <div class="content">{{project.summary}}</div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    props: ['project']
}
</script>

<style scoped>
.project-listing {
    /* Flexbox rules */
    display: flex;
    flex-direction: column;
    /* General spacing rules */
    margin: 2em;
}
</style>