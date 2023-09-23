<template>
  <header class="header">
  <nav class="main-nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/resume">Resume</router-link>
  </nav>
  <router-view/>
  </header>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Inclusive+Sans:wght@300;400&display=swap');

#app {
  font-family: Inclusive Sans, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #33a5de;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.header {
  display: flex;
}
</style>
