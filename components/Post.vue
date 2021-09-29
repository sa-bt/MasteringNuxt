<template>
    <div style="padding: 10px; margin: 10px;font-weight: bolder;background-color: orange">
        <NuxtLink :to="`/posts/${post.id}`"  >
            {{post.title}}
        </NuxtLink>
        <br>
    </div>
</template>

<script>
    export default {
        name: "Post",
        props: {
            post: {
                required: true,
                type: Object
            }
        }
    }
</script>

<style scoped>

</style>