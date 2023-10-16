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
  background-color: #60caff;
  background: linear-gradient(to bottom, #3498db, #2980b9);
  overflow: hidden;
  border-bottom: 2px;
  border-bottom-style: groove;
}

#picture-name-container {
  display: flex;
  flex-direction: column;
  background-color: #60caff;
  padding-top: 20px;
}

#portrait {
  height: 200px;
  margin: 5px;
  margin-bottom: 0;
  padding-bottom: 0;

}

#my-name {
  display: flex;
  justify-content: center;
  font-size: 36px;
  margin: 1px;
  padding: 1px;
  color: black;
  text-decoration: underline;

}

#nav-area {
  display: none;
}
</style>