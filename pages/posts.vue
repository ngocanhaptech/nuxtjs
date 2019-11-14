<template>
  <div class="container-main">
    <div>
      <h1>{{ title }}</h1>
      <div class="content">
          {{ body }}
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  layout: 'blog',
  asyncData ({ query, params, error }) {
    const id = query.id || '1'
    if (process.server) {
        //use route object
        console.log(params)
        //directly use params
        console.log(query.id)
    }
    return axios.get('https://jsonplaceholder.typicode.com/posts/' + id)
      .then((res) => {
        return { title: res.data.title, body: res.data.body }
      })
      .catch((e) => {
        error({ statusCode: 404, message: 'Post not found' })
      })
  }
}
</script>
