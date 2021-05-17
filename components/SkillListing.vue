<template>
    <div class="skill-listing">
        <div>{{skill.name}}</div>
        <div>{{skill.summary}}</div>
    </div>
</template>

<script>
export default {
    props: ['skill']
}
</script>