<template>
  <div id="footer-container">
    <nav id="nav-bar">
      <ul>
        <li>
          <router-link v-bind:to="{ name: 'home' }">
            <img src="../assets/icons8-home-50.png" id="home" />
            <p class="icon-text">Welcome</p>
          </router-link>
        </li>
        <li>
          <router-link v-bind:to="{name: 'about'}">
            <img src="../assets/icons8-about-me-50(2).png" id="marker" />
            <p class="icon-text">About Me</p>
          </router-link>
        </li>
        <li>
          <a @click="openPDF" style="cursor: pointer;">
            <img src="../assets/icons8-export-pdf-50.png" id="trophy" />
            <p class="icon-text">Resume</p>
            </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import resumePDF from "@/assets/Nicholas Marson Resume.pdf";

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
    openPDF() {
      const pdfWindow = window.open(resumePDF, "_blank");
      if (pdfWindow) {
        pdfWindow.focus();
      } else {
        alert("Please allow pop-ups for this website to view the PDF.");
      }
    },
  },
};
</script>

<style scoped>
img {
  width: 40px;
  height: auto;
  padding: 0;
  margin: 0;
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

  
}

nav ul {
  list-style: none;
  margin: 5;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  overflow: hidden;
}

nav ul li {
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


#footer-container a:hover {
  cursor: pointer;
}
</style>
