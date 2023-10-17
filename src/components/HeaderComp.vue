<template>
<div id="header-comp">

  <title-picture name="Nicholas Marson"/>
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
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #60caff;
  background: linear-gradient(to bottom, #3498db, #2980b9);
  border-bottom: 2px;
  border-bottom-style: groove;
  padding-top: 10px;
  padding-bottom: 20px;
  flex: 1;
}

#nav-area {
  display: none;
}
</style>