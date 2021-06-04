<template>
    <div>
        <div class="open-sans">{{project.name}}</div>
        <div class="montserrat">{{project.summary}}</div>
        <nuxt-content :document="project" class="montserrat"/>
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const project = await $content('portfolio/projects', params.slug).fetch();

        return {
            project
        }
    }
}
</script>