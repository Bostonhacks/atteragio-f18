<template>
  <div id="app">    
    <div class="navContain">
      <b-navbar fixed="top" id="nav">
          <router-link to="/">Home</router-link> |
          <router-link to="/faq">FAQ</router-link> |
          <router-link to="/schedule">Schedule</router-link> |
          <router-link to="/map">Map</router-link> |
          <router-link to="/resources">Resources</router-link> |
          <router-link to="/workshops">Workshops</router-link> |
          <router-link to="/prizes">Prizes</router-link>
      </b-navbar>
      <router-view/>
    </div>
    
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto:300,700');

body,html{
  padding-top: 9vw;
  width: 100%;
  height: 100vh;
  background-color:#a73d59;

  background-image: linear-gradient(
    to bottom,
    hsl(243, 45.45%, 25.88%) 0%,
    hsl(244.69, 45.23%, 25.91%) 10.8%,
    hsl(249.68, 44.51%, 26.01%) 21%,
    hsl(257.48, 43.27%, 26.18%) 30.8%,
    hsl(267.68, 41.51%, 26.42%) 40%,
    hsl(280.2, 39.26%, 26.72%) 48.6%,
    hsl(295.36, 36.56%, 27.09%) 56.7%,
    hsl(311.31, 38.26%, 29.66%) 64.1%,
    hsl(323.01, 41.05%, 33.21%) 71%,
    hsl(331.84, 43.23%, 36.98%) 77.2%,
    hsl(338.8, 44.94%, 40.92%) 82.7%,
    hsl(344, 46%, 45%) 87.6%,
    hsl(349.23, 47.38%, 49.3%) 91.8%,
    hsl(353.29, 55.98%, 53.71%) 95.3%,
    hsl(356.85, 68.33%, 58.26%) 98%,
    hsl(0, 84%, 63%) 100%
  );
}


#app {
  
  font-family: "Roboto", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  font-size: 1.5vw;
}



#nav {
  background-color: #6b6691;
  width: 100%;
  height: 5vw;

 
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
