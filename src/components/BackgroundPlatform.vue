<template>
  <div class="background-platform">
    <div class="upper-cover cover"></div>
    <div class="left-cover cover"></div>
    <div class="right-cover cover"></div>
    <div class="bottom-cover cover"></div>
  </div>
</template>

<script>
export default {
  name: 'background-platform',
  created () {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll (e) {
      console.log('hey scroll', e)
    }
  }
}
</script>

<style>

</style>
