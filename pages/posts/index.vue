<template>
  <div>
    <h1>Posts</h1>
    <post
      v-for="post in posts"
      :id="post.id"
      :key="post.id"
      :title="post.title"
    />
  </div>
</template>

<script>
import axios from 'axios'
import Post from '@/components/Post'

export default {
  components: {
    Post
  },
  data () {
    return {
      posts: []
    }
  },
  async created () {
    try {
      const res = await axios.get('https://jsonplaceholder.typicode.com/posts')
      this.posts = res.data
    } catch (error) {
      console.log(error)
    }
  }
}
</script>
