<template>
    <div>
        {{skill}}
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