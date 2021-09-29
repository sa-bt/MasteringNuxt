<template>
    <div style="padding: 10px; margin: 10px;font-weight: bolder;background-color: azure;text-align: center;padding: 15px">
        <img src="/images/icons/title.svg"  width="20" height="20" style="vertical-align: middle; margin-right:5px" alt="">Title: {{post.title}}
        <br>
        <img src="/images/icons/body.svg"  width="20" height="20" style="vertical-align: middle; margin-right:5px" alt="">Body: {{post.body}}
    </div>
</template>

<script>
    import posts from "~/data/posts"

    export default {
        name: "_id",
        data() {
            return {
                post: {}
            }
        }, created() {
            const post = posts.find((post) => post.id == this.$route.params.id)
            this.post = post
        }
    }
</script>

<style scoped>

</style>