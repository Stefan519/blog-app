<template>
    <div>
        <div v-bind:key="blog.id" v-for="blog in blogs">
            <BlogItem v-bind:blog="blog"/>
        </div>    
    </div>
</template>

<script>
import BlogItem from './BlogItem'

export default {
    name: 'BlogList',
    components: {
        BlogItem
    },
    props: ["blogs"]
}
</script>

<style>

</style>