<template>
    <div class="project-listing">
        <nuxt-link :to="'/project/' + project.slug">
            <div>{{project.name}}</div>
            <div>{{project.summary}}</div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    props: ['project']
}
</script>