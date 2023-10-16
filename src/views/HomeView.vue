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
  overflow: none;
}
#footer-comp {
  height: 15%;
}
</style>
