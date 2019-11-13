<template>
    <div class="header">
      <div class="container flex">
        <logo />
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
