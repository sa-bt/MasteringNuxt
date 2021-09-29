<template>
    <div>
        <div v-for="photo in photos" :key="photo.id">
            <Item :photo="photo" />
        </div>
    </div>
</template>

<script>
    import photos from '~/data/images'

    export default {
        name: "index",
        data() {
            return {
                photos: photos
            }
        }
    }
</script>

<style scoped>

</style>