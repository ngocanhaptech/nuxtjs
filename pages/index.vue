<template>
  <div class="container-main justify-content-center align-items-center text-center">
    <div>
      <h1 class="title">
        Index page
      </h1>
      <h2 class="subtitle">
        BizFlyCloud stop innovation.
      </h2>
      <div class="content">Content home page</div>
    </div>
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Home page',
      meta: [
        { hid: 'description', name: 'description', content: 'Home page descriptions ' }
      ]
    }
  }
}
</script>
<style>
.text-center {
  text-align: center;
}
.container-main {
  margin: 0 auto;
  min-height: calc(100vh - 80px);
  display: flex;
}
.justify-content-center {
  justify-content: center;
}
.align-items-center {
  align-items: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
