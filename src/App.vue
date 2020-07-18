<template>
  <div id="app">
    <div>
      <Header />
    </div>
    <div>
      <BlogList v-bind:blogs="blogs"/>
    </div>
    <div>
      <Sidebar v-bind:blogs="blogs"/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header'
import BlogList from './components/BlogList'
import Sidebar from './components/Sidebar'

export default {
  name: 'App',
  components: {
    Header,
    BlogList,
    Sidebar
  },
  data() {
    return {
      blogs: [
        {
          id: 1,
          title: "Marlons Blog",
          text: "great blog",
          hashtag: "#hamburg #2liga"
        },
        {
          id: 2,
          title: "Stefans Blog",
          text: "awesome blog",
          hashtag: "#bielefeld #1liga"
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
