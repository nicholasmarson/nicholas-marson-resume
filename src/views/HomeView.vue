<template>
<div id="home-view">
  <header-comp/>
  <greeting />
  <footer-comp />
</div>
 
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/HeaderComp.vue'
import Greeting from '@/components/Greeting.vue'
import FooterComp from '@/components/FooterComp.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderComp,
    Greeting,
    FooterComp
  }
}
</script>

<style>
#home-view {
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
}

#header-comp {
  height: 31%;
}

#greeting-message {
  height: 59%;
}

#footer-container {
  height: 10%;
}



@media (min-width: 429px) and (min-height: 927px) {
#header-comp {
  display: grid;
  grid-template-columns: 1fr 1fr;
  background-color: #60caff;
  grid-template-areas:
  "title nav"
  ;
  border: 3px solid #216dc9;
}

#picture-name {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  text-decoration: underline;
}

#portrait {
  height: 100px;
  margin: 5px;
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
}
</style>
