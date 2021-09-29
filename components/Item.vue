<template>
    <div>
        <img :src="photo.thumbnailUrl" alt="" style="width: 300px">
        <br>
        {{photo.title}}
        <br>
    </div>
</template>

<script>
    export default {
        name: "Item",
        props: {
            photo: {
                required: true,
                type: Object
            }
        }
    }
</script>

<style scoped>

</style>