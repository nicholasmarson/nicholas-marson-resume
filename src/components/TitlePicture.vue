<template>
  <div>
    <img id="portrait" src="@/images/circle-portrait.png" alt="Picture of me"/>
    {{ name }}
  </div>
</template>

<script>
export default {
  props: {
    name: String
  }
  
}
</script>

<style scoped>

div {
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

</style>