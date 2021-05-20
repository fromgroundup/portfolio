<template>
    <div>
        <div class="heading">{{skill.name}}</div>
        <div class="content">{{skill.summary}}</div>
        <nuxt-content :document="skill" class="content"/>
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