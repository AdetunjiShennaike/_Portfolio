<template>
  <div id="app">
    <nav class="sideBar" id="sideBar">
      <Navigation />
      <SocialMedia />
     </nav>
    <div class="Page">
      <router-view/>
      Icons by <a href="https://www.flaticon.com/authors/mynamepong" title="mynamepong">mynamepong</a>
      <br/>Icons by <a href="https://www.flaticon.com/authors/freepik" title="Freepik">Freepik</a>
    </div>
  </div>
</template>
<script>
import Navigation from '@/components/nav/Navigation'
import SocialMedia from '@/components/nav/SocialMedia'
export default {
  components: {
    Navigation,
    SocialMedia
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.Page {
  height: 100%;
  width: 100%;
  position: absolute;
}
/* Navigation styling */
#sideBar {
  background: #10fd08;
  height: 100%;
  width: 50px;
  position: absolute;
  right: 0;
  top: 0;
  z-index: 3;
  min-height: 600px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  white-space: nowrap;
}
#nav {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: space-evenly;
}
#social-nav {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: space-evenly;
}
.navIcon {
  height: auto;
  width: 35px;
}
</style>
