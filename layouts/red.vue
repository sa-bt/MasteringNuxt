<template>
    <div>
        <header style="background-color: red">
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/posts/">Posts</NuxtLink>
        </header>
        <Nuxt/>
    </div>
</template>

<script>
    export default {
        name: "red"
    }
</script>

<style scoped>

</style>