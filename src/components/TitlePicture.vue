<template>
  <div id="picture-name-container">
    <img id="portrait" src="@/images/circle-portrait.png" alt="Picture of me"/>
    <p id="my-name">{{ name }} </p>
  </div>
</template>

<script>
export default {
  props: {
    name: String
  }
  
}
</script>

<style>
</style>