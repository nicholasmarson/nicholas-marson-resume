<template>
  <div id="footer-container">
    <nav>
      <ul>
        <li>
          <router-link v-bind:to="{ name: 'home' }">
            <img src="../assets/home.png" id="home" />
          </router-link>
        </li>
        <li>
          <router-link v-bind:to="{name: 'about'}">
            <img src="../assets/marker.png" id="marker" />
          </router-link>
        </li>
        <li>
          <router-link v-bind:to="{ name: 'resume' }">
            <img src="../assets/trophy.png" id="trophy" />
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
  display: flex;
  justify-content: center;
  align-items: center;
}

nav ul {
  list-style: none;
  margin: 5;
  padding: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100vw;
}

nav ul li {
  font-size: 16px;
  text-align: center;
  flex: 1;
  margin: 0, 10px;
}
</style>