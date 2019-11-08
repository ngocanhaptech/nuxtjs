<template>
  <div>
    <div class="top flex justify-between items-center">Top content</div>
    <div class="header">
      <div class="container flex">
        <ul class="navigation">
          <li>
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/about">About</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/team">Team</nuxt-link>
          </li>  
          <li>
            <nuxt-link to="/blog">Blog</nuxt-link>
          </li>        
        </ul><!-- /.navigation -->
      </div> <!-- /.container -->
    </div>
    <nuxt />
  </div>
</template>

<style>
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
</style>
