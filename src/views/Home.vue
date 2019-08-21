<template>
  <!-- <div class="home"> -->
    <div class="main-page">
      <!-- <div class="square"></div> -->
    <Home-Component/>
    <Art-One></Art-One>
    <About/>
      <!-- <div class="text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore sed error saepe veniam voluptatem neque, earum ullam numquam. Alias ad aspernatur natus, fugiat possimus similique reprehenderit unde voluptates sunt facere.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore sed error saepe veniam voluptatem neque, earum ullam numquam. Alias ad aspernatur natus, fugiat possimus similique reprehenderit unde voluptates sunt facere.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore sed error saepe veniam voluptatem neque, earum ullam numquam. Alias ad aspernatur natus, fugiat possimus similique reprehenderit unde voluptates sunt facere.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore sed error saepe veniam voluptatem neque, earum ullam numquam. Alias ad aspernatur natus, fugiat possimus similique reprehenderit unde voluptates sunt facere.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore sed error saepe veniam voluptatem neque, earum ullam numquam. Alias ad aspernatur natus, fugiat possimus similique reprehenderit unde voluptates iil
      </div> -->
    </div>
  <!-- </div> -->
</template>

<script>
// @ is an alias to /src
import HomeComponent from '@/views/HomeComponent.vue'
import ArtOne from '@/views/Art1.vue'
import About from '@/views/About.vue'

export default {
  name: 'home',
  components: {
    HomeComponent,
    About,
    ArtOne
  },
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
<style lang="scss" scoped>
.main-page {
  width: 100vw;
  height: 100%;
  display: flex;
  justify-content: center;
  // align-items: flex-start;
  align-items: center;
  position: relative;
  .square {
    height: 100px;
    width: 100px;
    background-color: black;
    position: fixed;
    bottom: 0;
  }
}
</style>

