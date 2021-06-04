<template>
    <div>
        <div class="open-sans">{{skill.name}}</div>
        <div class="montserrat">{{skill.summary}}</div>
        <nuxt-content :document="skill" class="montserrat"/>
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const skill = await $content('portfolio/skills', params.slug).fetch();

        return {
            skill
        }
    }
}
</script>