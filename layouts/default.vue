<template>
  <div>
    <top />
    <header-component>
      <navigation />
    </header-component>
    <nuxt />
  </div>
</template>

<script>
import Logo from '@/components/Logo'
import Top from '@/components/Top'
import HeaderComponent from '@/components/Header'
import Navigation from '@/components/Navigation'

export default {
  components: {
    Logo,
    Top,
    HeaderComponent,
    Navigation
  },
  mounted () {
    // const scriptMain = document.getElementById('mega_menu_main_js')
    // setTimeout(() => {
    //   scriptMain && scriptMain.setAttribute('src', 'js/main.js')
    // }, 3000)
  },
  head () {
    return {
      link: [
        { rel: 'stylesheet', href: 'css/style.css' }
      ],
      script: [
        // { src: 'js/jquery-2.1.1.js', rel: 'preload' },
        // { src: 'js/jquery-2.1.1.js', body: true },
        // { src: 'js/jquery.mobile.custom.min.js', rel: 'preload' },
        // { src: 'js/jquery.mobile.custom.min.js', body: true },
        // { src: 'js/modernizr.js', rel: 'preload' },
        // { src: 'js/modernizr.js', body: true },
        // Mega menu
        // { src: 'js/main.js', rel: 'preload' },
        // { src: '', body: true, id: 'mega_menu_main_js' }
      ]
    }
  },
  // Scroll to the top before rendering the page
  scrollToTop: true
}
</script>
