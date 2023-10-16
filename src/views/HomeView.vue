<template>

  <header-comp/>
  <greeting />
  
 
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/HeaderComp.vue'
import Greeting from '@/components/Greeting.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderComp,
    Greeting
  }
}
</script>

<style>

</style>
