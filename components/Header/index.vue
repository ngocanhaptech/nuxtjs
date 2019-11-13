<template>
    <div class="header">
      <div class="container flex justify-content-between">
        <nuxt-link to="/"><logo /></nuxt-link>
        <slot />
      </div> <!-- /.container -->
    </div>
</template>

<script>
import Logo from '@/components/Logo'

export default {
  components: {
    Logo
  }
}
</script>
