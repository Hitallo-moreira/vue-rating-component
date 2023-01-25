<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/sucess">Sucess</router-link>
    <Footer />
  </nav>
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
<style>
  * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Overpass', sans-serif;
  }

  body {
    height: 100vh;
    background-color: #121417;
  }
</style>
