<template>
  <div>
    <top />
    <header-component>
      <navigation />
    </header-component>
    <mega />
    <nuxt />
  </div>
</template>

<script>
import Logo from '@/components/Logo'
import Top from '@/components/Top'
import HeaderComponent from '@/components/Header'
import Mega from '@/components/Mega'
import Navigation from '@/components/Navigation'

export default {
  components: {
    Logo,
    Top,
    HeaderComponent,
    Mega,
    Navigation
  },
  mounted () {
    const scriptMain = document.getElementById('mega_menu_main_js')
    setTimeout(() => {
      scriptMain && scriptMain.setAttribute('src', 'js/main.js')
    }, 3000)
  },
  head () {
    return {
      link: [
        { rel: 'stylesheet', href: 'css/style.css' }
      ],
      script: [
        { src: 'js/jquery-2.1.1.js' },
        { src: 'js/jquery.mobile.custom.min.js' },
        { src: 'js/modernizr.js' },
        // Mega menu
        { src: 'js/main.js', rel: 'preload' },
        { src: '', body: true, id: 'mega_menu_main_js' }
      ]
    }
  },
  // Scroll to the top before rendering the page
  scrollToTop: true
}
</script>
