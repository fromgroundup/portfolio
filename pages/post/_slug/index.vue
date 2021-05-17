<template>
    <div class="post">
        <div class="heading">{{post.title}}</div>
        <div class="heading">{{post.subtitle}}</div>
        <nuxt-content :document="post" class="content"/>
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