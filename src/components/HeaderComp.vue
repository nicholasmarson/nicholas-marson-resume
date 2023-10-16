<template>
<div id="header-comp">

  <title-picture id="title-area" name="Nicholas Marson"/>
  {{ name }}
  <navigation id="nav-area"/>
  
  </div>
</template>

<script>
import Navigation from './Navigation.vue'
import TitlePicture from './TitlePicture.vue'

export default {
  props: {
    name: String,
  },
  components: { 
    TitlePicture,
    Navigation 
    },

}
</script>

<style>
#header-comp {
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
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: 5%;
}

#title-area {
  grid-area: title;
  display: flex;
  justify-content: flex-start;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

</style>