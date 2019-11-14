<template>
  <div class="container-main">
    <div>
      <h1>Blog page</h1>
      <div class="content">
        <div class="item-post" v-for="item in list" :key="item.id">
            <h3><nuxt-link :to="'/posts?id=' + item.id">{{ item.title }}</nuxt-link></h3>
            <p>{{ item.body }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  layout: 'blog',
  asyncData ({ params, error }) {
    return axios.get('https://jsonplaceholder.typicode.com/posts')
      .then((res) => {
        console.log('getList', res.data)
        return { list: res.data }
      })
      .catch((e) => {
        error({ statusCode: 404, message: 'Post not found' })
      })
  }
}
</script>
