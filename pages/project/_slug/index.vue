<template>
    <div>
        <div class="heading">{{project.name}}</div>
        <div class="content">{{project.summary}}</div>
        <nuxt-content :document="project" class="content"/>
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