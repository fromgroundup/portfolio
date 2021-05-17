<template>
    <div class="project-listing">
        <div>{{project.name}}</div>
        <div>{{project.summary}}</div>
    </div>
</template>

<script>
export default {
    props: ['project']
}
</script>