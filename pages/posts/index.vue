<template>
    <div style="width: 100%; text-align: center">
        <div v-for="post in posts" :key="post.id" style="padding: 10px; margin: 10px;font-weight: bolder;background-color: orange">
            <Post :post="post" />
        </div>
    </div>
</template>

<script>
    import posts from '~/data/posts'

    export default {
        name: "index",
        head(){
            return{
                title:'HomePage',
                meta:[{
                    name:'description',
                    content:'This is a homepage',
                    hid:'description'
                }]
            }
        },
        data() {
            return {
                posts: posts
            }
        }
    }
</script>

<style scoped>

</style>