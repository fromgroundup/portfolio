<template>
    <div>
        <ProjectListing v-for="work in projects" :project="work" :key="work.createdAt"/>
        <SkillListing v-for="talent in skills" :skill="talent" :key="talent.createdAt"/>
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const projects = await $content('portfolio/projects').fetch()
        const skills = await $content('portfolio/skills').fetch()

        return {
            projects, skills
        }
    }
}
</script>