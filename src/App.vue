<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    
    <router-view/>
  </div>
</template>

<style lang="scss">
@import './assets/scss/_app';

#app {
  // font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 10000px;
  height: 100%;
  height: 100vh;
  overflow: hidden;
  /* 005 Young Passion: */
  background-image: linear-gradient(90deg, #B12A5B 0%, #CF556C 25%, #FF8C7F 63%, #FF8177 100%);
  /* 126 Colorful Peach: */
  background-image: linear-gradient(90deg, #EC8C69 0%, #ED6EA0 100%);
  /* 070 Aqua Splash: */
  background-image: linear-gradient(-160deg, #13547A 0%, #80D0C7 100%);
}
body{
  &::-webkit-scrollbar {
    width: 20px;
    height: 100px;
    display: none;
    background-color: transparent;
    // background-image: linear-gradient(-160deg, #13547A 0%, #80D0C7 100%);
    position: absolute;
    bottom: 0;
} 
&::-webkit-scrollbar-thumb {
  background-color: #000000;
}
&::-webkit-scrollbar-track {
  display: none;
  -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
    background-color: transparent;
      // background-image: linear-gradient(-160deg, #13547A 0%, #80D0C7 100%);
}

}

#nav {
  padding: 30px;
  position: fixed;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
