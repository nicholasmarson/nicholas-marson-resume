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

@media (min-width: 429px) and (min-height: 927px) {
#home-view {
  height: 100vh;
}

#header-comp {
  height: 13%;
  margin: 0;
  padding: 0;
}

#about-me {
  height: 90%;
}

#picture-name-container {
  padding: 0;
  margin: 5px;
}

#portrait {
  height: 100px;
  margin: 5px;
}
}
</style>
