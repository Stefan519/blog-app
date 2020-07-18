<template>
    <div>
        <h1>{{ blog.title }}</h1>
        <p>{{ blog.text }}</p>
        <p>{{ blog.hashtag }}</p>
    </div>
</template>

<script>
export default {
    name: 'BlogItem',
    props: ["blog"]
}
</script>

<style>

</style>