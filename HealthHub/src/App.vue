<script>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
export default {

  data () {
    return {
      show: false,
      showLogin: true
    }
  },
  methods: {
    openMain() {
      this.show = true
      this.showLogin = false
    }
  },
  components: {Navbar}
}
</script>

<template>
  <Navbar/>

  <router-view/>
</template>

<style scoped>

</style>
