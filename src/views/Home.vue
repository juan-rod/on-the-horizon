<template>
  <div class="main-page background-platform">
    <Intro-Details/>
  </div>
</template>

<script>
// @ is an alias to /src
import IntroDetails from '@/views/IntroDetails.vue'
import BackgroundPlatform from '@/components/BackgroundPlatform.vue'
import TeachingPhoto from '@/components/TeachingPhoto.vue'
import About from '@/views/About.vue'

export default {
  name: 'home',
  components: {
    IntroDetails,
    BackgroundPlatform,
    About,
    TeachingPhoto
  },
  // created () {
  //   window.addEventListener('scroll', this.handleScroll);
  // },
  // destroyed () {
  //   window.removeEventListener('scroll', this.handleScroll);
  // },
  // methods: {
  //   handleScroll (e) {
  //     console.log('hey scroll', e)
  //   }
  // }
}
</script>
<style lang="scss" scoped>

</style>

