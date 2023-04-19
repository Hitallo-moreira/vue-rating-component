<template>
  <Footer />
  <router-view/>
</template>
<script>
import Footer from './components/Footer/Footer.vue'

export default {
  name: 'Home',
  components: {
    Footer
  }
}
</script>
<style lang="scss">
  @import "@/assets/scss/_variables.scss";
  
  * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Overpass', sans-serif;
  }

  body {
    background-color: $very-dark-blue;
  }
</style>
