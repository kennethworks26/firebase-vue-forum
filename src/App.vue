<template>
  <div id="app">
    <TheNavBar />
    <div class="container">
      <router-view />
    </div>
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar'
export default {
  components: {
    TheNavBar
  },
  mounted () {
    console.log(this.$store.state)
  }
}
</script>

<style>
@import "assets/css/style.css";
</style>
