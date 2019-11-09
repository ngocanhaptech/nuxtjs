<template>
  <div>
    <div class="top flex justify-between items-center">Top content</div>
    <div class="header">
      <div class="container flex">
        <nav />
      </div> <!-- /.container -->
    </div>
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
import Nav from '@/components/Navigation'
export default {
  components: {
    Nav
  }
}
</script>

<style>
.main { 
    flex-grow: 1;
}
.sidebar { 
    margin-left: auto;
    grid-column: 10;
    min-width: 220px;
}
.navigation {
  margin: 0;
  padding: 0;
  list-style-type: none;
}
.navigation li {
  display: inline-block;
}
.navigation li a{
  display: inline-block;
  padding: 5px 12px;
}
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
.flex {
  display: flex;
}
.justify-between {
  justify-content: center;
}
.items-center {
  align-items: center;
}
.container {
  max-width: 1200px;
  margin: auto;
}
body {
  padding-top: 35px;
}
.top {
  border-bottom: 1px solid #eaeaea;
  min-height: 34px;
  background: #35495e;
  color: #ccc; 
  padding: 0 15px;
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
}
.list-unstyled {
    margin: 0;
    padding: 0;
    list-style-type: none;
}
</style>
