<template>
<div id="about-view">
  <header-comp />
  <about-me />
  <footer-comp />
  </div>
</template>

<script>
import HeaderComp from "@/components/HeaderComp.vue";
import FooterComp from "@/components/FooterComp.vue";
import AboutMe from '@/components/AboutMe.vue';
export default {
  components: {
    HeaderComp,
    FooterComp,
    AboutMe,
  },
};
</script>

<style>
#about-view {
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
}

#header-comp {
  height: 30%;
}

#about-me {
  height: 60%;
}

#footer-container {
  height: 10%;
}
</style>
