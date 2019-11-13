<template>
  <ul class="navigation">
    <li>
      <nuxt-link to="/">Home</nuxt-link>
    </li>
    <li>
      <nuxt-link to="/about">
        Products
        <svg data-icon="chevron-down" width="12" height="12" viewBox="0 0 20 20" class="css-wh3yq6" style="fill: rgb(53, 73, 94);"><path d="M16 6c-.28 0-.53.11-.71.29L10 11.59l-5.29-5.3a1.003 1.003 0 0 0-1.42 1.42l6 6c.18.18.43.29.71.29s.53-.11.71-.29l6-6A1.003 1.003 0 0 0 16 6z" fill-rule="evenodd"></path></svg>
      </nuxt-link>
      <ul class="sub-menu">
        <li v-for="item in menu" :key="'menu-item-' + item.title">
          <div class="text flex items-center">
            <svg data-icon="icon-protocols" width="18" height="18" viewBox="0 0 24 24" class="css-w90s2p"><path d="M20.63,17.45a.48.48,0,0,0-.48.47V22a.6.6,0,0,1-.6.59H1.8A.6.6,0,0,1,1.2,22V18.34H13.13a.48.48,0,0,0,.47-.48.47.47,0,0,0-.47-.47H1.2V12.47H6a.47.47,0,1,0,0-.94H1.2V6.61H13.13a.47.47,0,0,0,.47-.47.48.48,0,0,0-.47-.48H1.2V2a.58.58,0,0,1,.06-.26.47.47,0,0,0-.21-.63.46.46,0,0,0-.63.21A1.46,1.46,0,0,0,.25,2V22A1.55,1.55,0,0,0,1.8,23.54H19.55A1.54,1.54,0,0,0,21.1,22V17.92A.47.47,0,0,0,20.63,17.45Z" fill-rule="evenodd"></path><path d="M19.55.46H3.45a.47.47,0,1,0,0,.94h16.1a.6.6,0,0,1,.6.59V6.08a.48.48,0,0,0,.48.47.47.47,0,0,0,.47-.47V2A1.54,1.54,0,0,0,19.55.46Z" fill-rule="evenodd"></path><path d="M8.37,12a.47.47,0,0,0,.47.47h9a.47.47,0,1,0,0-.94h-9A.47.47,0,0,0,8.37,12Z" fill-rule="evenodd"></path><path d="M20.67,15.08A3.08,3.08,0,1,1,23.75,12,3.08,3.08,0,0,1,20.67,15.08Zm0-5.45A2.37,2.37,0,1,0,23,12,2.38,2.38,0,0,0,20.67,9.63Z" fill-rule="evenodd"></path></svg>
            <span>{{ item.title }}</span>
          </div>
          <div class="des">{{ item.description }}</div>
        </li>
      </ul>
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
</template>

<script>
export default {
  data() {
    return {
      menu: [
        { title: 'BizFly Cloud Server', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly CDN', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Business Email', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Load Balancer', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Simple Storage', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Pre-built application', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly VPN', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Container Registry', description: 'Power your growth and analytics tools with one API' },
        { title: 'BizFly Call Center', description: 'Power your growth and analytics tools with one API' }
      ]
    }
  }
}
</script>
