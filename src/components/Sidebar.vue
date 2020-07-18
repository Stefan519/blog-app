<template>
    <div>
        <div v-bind:key="blog.id" v-for="blog in blogs">
            <h1>{{ blog.hashtag }}</h1>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Sidebar',
    props: ['blogs']
}
</script>

<style>

</style>