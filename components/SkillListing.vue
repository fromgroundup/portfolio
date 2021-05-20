<template>
    <div class="skill-listing">
        <nuxt-link :to="'/skill/' + skill.slug">
            <div>{{skill.name}}</div>
            <div>{{skill.summary}}</div>
        </nuxt-link>
    </div>
</template>

<script>
export default {
    props: ['skill']
}
</script>