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
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&display=swap');

:root {
  --big-border: 6px solid black;
  --sml-border: 2px solid black;
  --red-color: #eb4034;
  --active: #36d97a;
  --blue: #2980b9;
  --font-main: #404040;
  --main-grey: #dedede;
}

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}
</style>
