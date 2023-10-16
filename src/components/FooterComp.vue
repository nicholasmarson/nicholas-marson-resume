<template>
  <div id="footer-container">
    <nav id="nav-bar">
      <ul>
        <li>
          <router-link v-bind:to="{ name: 'home' }">
            <img src="../assets/home.png" id="home" />
            <p class="icon-text">Welcome</p>
          </router-link>
        </li>
        <li>
          <router-link v-bind:to="{name: 'about'}">
            <img src="../assets/marker.png" id="marker" />
            <p class="icon-text">About Me</p>
          </router-link>
        </li>
        <li>
          <router-link v-bind:to="{ name: 'resume' }">
            <img src="../assets/trophy.png" id="trophy" />
            <p class="icon-text">Resume</p>
          </router-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "footer-comp",
  data() {
    return {
      isDropdownOpen: false,
    };
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
  },
};
</script>

<style scoped>
img {
  width: 30px;
  height: auto;
}

#footer-container {
  width: 100%;
  background-color: #60caff;
  background: linear-gradient(to bottom, #3498db, #2980b9);
  border-top: 2px;
  border-top-style: solid;
  border-top-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0%;
  padding: 0%;
}

nav {
  height: 100%;
  width: 100%;
  padding-top: 2.5%;
  
}

nav ul {
  list-style: none;
  margin: 5;
  padding: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100vw;
  overflow: hidden;
}

nav ul li {
  font-size: 16px;
  text-align: center;
  flex: 1;

}


.icon-text {
    text-decoration: none;
    color: black;
    padding: 0;
    margin: 0;
    font-size: 8px;
}
</style>