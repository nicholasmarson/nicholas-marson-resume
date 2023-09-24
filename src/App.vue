<template>
  
  <header>
    <TitlePicture id="title-area" name="Nicholas Marson"/>
    <Navigation id="nav-area"/>
  </header>
  
  <div>
    <router-view id="main-area"/>
  </div>

</template>

<script>
import Navigation from './components/Navigation.vue'
import TitlePicture from './components/TitlePicture.vue';

export default {
  components: {
    Navigation,
    TitlePicture
}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Inclusive+Sans:wght@300;400&display=swap');

#app {
  font-family: Inclusive Sans, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

header {
  display: grid;
  grid-template-columns: 1fr 1fr;
  background-color: #60caff;
  grid-template-areas:
  "title nav"
  ;
  border: 3px solid #216dc9;
}

nav a.router-link-exact-active {
  color: #ffffff;
}

#nav-area {
  grid-area: nav;
}

#title-area {
  grid-area: title;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
