<template>
  <div class="home-page">
    <div class="upper-cover cover"></div>
    <div class="left-cover cover"></div>
    <div class="right-cover cover"></div>
    <div class="bottom-cover cover"></div>
    <div class="main-heading">
      <div class="heading">
        <h1 class="heading-name">juan rodriguez</h1>
        <h1 class="heading-title">portfolio site thing</h1>
      </div>
      <div class="main">
        <h3>Juan Rodriguez is an Austin-based <span> Software Developer </span> at L7 Informatics.</h3>
        <h3>Juan Rodriguez is an Austin-based <span> Web 101 Instructor </span> at Austin Coding Academy.</h3>
      </div>
    </div>
    <Art-One/>
    <About/>
  </div>
</template>

<script>
import ArtOne from '@/views/Art1.vue'
import About from '@/views/About.vue'

export default {
  name: 'home-component',
  components: {
    About,
    ArtOne
  }
}
</script>

<style lang="scss" scoped>

</style>
