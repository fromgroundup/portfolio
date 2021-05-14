<template>
    <div>
        <BlogPostListing v-for="post in posts" :preview="post" :key="post.path"/>
    </div>
</template>

<script>
export default {
    async asyncData({ $content, params }) {
        const posts = await $content('posts').only(['title', 'updatedAt', 'slug', 'subtitle']).fetch()

        return {
            posts
        }
    }
}
</script>