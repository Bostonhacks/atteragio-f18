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

body{
  padding-top: 9vw;
  width: 100%;
  height: 155vh;
  background-color:#a73d59;

  background-image: linear-gradient(
    to bottom,
    hsl(243, 47%, 25%) 0%,
    hsl(243.26, 46.43%, 24.91%) 13.8%,
    hsl(244.67, 46.23%, 24.93%) 26.4%,
    hsl(248.25, 45.7%, 25.01%) 38%,
    hsl(254.52, 44.68%, 25.15%) 48.4%,
    hsl(263.59, 43.09%, 25.37%) 57.7%,
    hsl(275.57, 40.85%, 25.69%) 66%,
    hsl(290.88, 37.97%, 26.11%) 73.3%,
    hsl(308.95, 38.24%, 28.23%) 79.7%,
    hsl(322.67, 41.38%, 32.25%) 85.1%,
    hsl(332.78, 43.77%, 36.63%) 89.6%,
    hsl(340.57, 45.6%, 41.33%) 93.3%,
    hsl(346.8, 46.99%, 46.33%) 96.1%,
    hsl(351.93, 51.26%, 51.62%) 98.2%,
    hsl(356.26, 65.21%, 57.16%) 99.4%,
    hsl(0, 84.13%, 62.94%) 100%
  );
}



#app {  
  font-family: "Roboto", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  font-size: 1.25vw;
  
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
