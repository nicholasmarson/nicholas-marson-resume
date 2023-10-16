<template>
  <div id="picture-name-container">
    <img id="portrait" src="@/images/IMG_4011.jpeg" alt="Picture of me"/>
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

<style scoped>
#portrait {
  border: 7px;
  border-style: solid;
  border-radius: 60%;
  border-color: rgb(0, 0, 0);
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
}

#my-name {
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
}

</style>