<template>
  <div class="">
    <Navbar></Navbar>
    <nuxt />
    <Footer></Footer>
  </div>
</template>

<style>
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
body{
    @apply bg-gray-100;
}
.font-serif{
  font-family:yale,TimesNewRoman,Times New Roman,Times,Baskerville,Georgia,serif;
}
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>
