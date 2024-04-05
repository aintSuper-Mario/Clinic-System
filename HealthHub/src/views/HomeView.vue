<template>
  <main>
    <Main />
    <Services />
    <Footer />
  </main>
</template>

<script>
import Main from '../components/Main.vue'
import Services from '../components/Services.vue'
import Footer from '../components/Footer.vue'
export default {
  components: {
    Main, Services, Footer
  }
}
</script>

<style scoped>
 main {
  background-image: url(../assets/images/aboutus1.jpg);
  background-size: cover;
  height: 600px;
 }
</style>
