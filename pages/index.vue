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
                photos: photos
            }
        }
    }
</script>

<style scoped>

</style>