<template>
  <div>
    <top />
    <header-component>
      <navigation />
    </header-component>
    <div class="container flex">
        <main class="main">
            <nuxt />
        </main>
        <aside class="sidebar">
            <h4>Post</h4>
            <ul class="list-unstyled">
                <li><nuxt-link to="/blogs/post1">Post title first</nuxt-link></li>
                <li><nuxt-link to="/blogs/post2">Post title second</nuxt-link></li>
                <li><nuxt-link to="/blogs/post3">Post title third</nuxt-link></li>
                <li><nuxt-link to="/blogs/post4">Post title fourth</nuxt-link></li>
                <li><nuxt-link to="/blogs/post5">Post title fifth</nuxt-link></li>
            </ul>
        </aside>
    </div>
  </div>
</template>
<script>
import Top from '@/components/Top'
import HeaderComponent from '@/components/Header'
import Navigation from '@/components/Navigation'
export default {
  head () {
    return {
      link: [
        { rel: 'stylesheet', href: 'css/style.css' }
      ]
    }
  },
  components: {
    Top,
    HeaderComponent,
    Navigation
  }
}
</script>
