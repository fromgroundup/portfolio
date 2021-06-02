<template>
    <div class="post">
        <div class="open-sans">{{post.title}}</div>
        <div class="open-sans">{{post.subtitle}}</div>
        <nuxt-content :document="post" class="montserrat"/>
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const post = await $content('posts', params.slug).fetch();
        return {
            post
        }
    }
}
</script>