<template>
  <div>
    <b-container fluid>
      <b-row align-h="end">
        <div style="margin-top: -1.5vw; margin-right: 10vw;">
          <div id="redot" style="margin-right: 1vh"></div><span style="font-size: 1.6vw; font-weight: 400;">Live</span>
        </div>
      </b-row>
    </b-container>
    
    <b-container fluid> 
        <b-row class="homeHead">
            <b-col>Flair</b-col>
            <b-col cols="6" id="heroText">
              <div >
                <p class="heroText"> Boston<span id="bolder">Hacks</span> 2018 </p>
                <p class="date">November 10 &#8211; November 11, 2018<br>
                775 Commonwealth Avenue, Boston University</p>
              </div>
            </b-col>
            <b-col>Flair</b-col>
        </b-row>
    </b-container>
    
    <b-container id="links" >
      <b-row id="links" class="links">
        <b-col cols="auto" md="4">
          <div>
            <img class="icon" src="../assets/Icons/wifi.svg"/>
          </div>
          
          <div>
            <p class="headInfo"><span id="bolder">Wifi</span></p>
            <p class="info"><span id="bolder">Network:</span> BU Event Guest</p>
            <p class="info"><span id="bolder">Password:</span> w!flP/ss%#rd</p>
          </div>
        </b-col>
       
        <b-col cols="auto" md="4">
          <div>
            <img class="icon" src="../assets/Icons/slack.svg"/>
          </div>
          <div>
            <p class="headInfo"><span id="bolder">Slack</span></p>
            <p class="info">Click here to join our Slack channel!</p>
            <p class="info">(link here)</p>
          </div>
        </b-col>
        
        <b-col cols="auto" md="4">
          <div>
            <img class="icon" src="../assets/Icons/link.svg"/>
          </div>
          
          <div>
            <p class="headInfo"><span id="bolder">Devpost</span></p>
            <p class="info">Click here for project submission</p>
            <p class="info">and prize info (link here)</p>
          </div>
        </b-col>
      </b-row> 
    </b-container>

    <b-container  style="margin-top: 15vw;">
        <hr>
        <p id="bolder">Thank you to our sponsors!</p>
    </b-container>

    <b-container fluid>
      <b-row style="padding: 3vw 5vw 0 5vw;">
        <b-col><img class="logo" src="../assets/Logos/Bose/BoseLogo.png"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/BUCS/BucsLogo.jpg"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/Giphy/giphyEngineeringLogo.jpg"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/Github/githubLogo.png"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/Google/googleLogo.png"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/ITG/itgWhiteLogo.png"/></b-col>
      </b-row>

      <b-row style="padding: 4vw 5vw 4vw 5vw;">
        <b-col><img class="logo" src="../assets/Logos/Liberty/libertyLogo.png"/></b-col>
        <b-col><img src="../assets/Logos/MassRobotics/massRoboLogo.png" style="height: 3vw;"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/OneDB/onedbLogo.svg"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/Raytheon/raytheonLogo.png"/></b-col>
        <b-col><img class="logo" src="../assets/Logos/RedHat/redhatLogo.png"/></b-col>
        <b-col></b-col>
      </b-row>

    </b-container>

  </div>
  
</template>

<script>
export default {
  name: "home",
  components: {}
};
</script>

<style lang="scss">


.heroText {
  color: white;
  font-family: "Roboto", Arial, Helvetica, sans-serif;
  font-weight: 300;
  font-size: 3.7vw;
}

.date{
  margin-top: 1vh;
  line-height: 1.75vw;
  font-weight: 300;
}

#bolder {
  font-weight: 700;
}

.homeHead{
  padding-top: 18vh;
} 

@media (max-width: 750px) {
  .homeHead {
    margin-top: -12vw;
  }
}

#links {
  padding-top: 8.5vw;
  margin-left: auto;
  margin-right: auto;
}

.links{
  width: 90%;
  margin: 0;
  text-align: start;
}


.icon {
  height: 2vw;
  width: 2vw;
  margin-bottom: 2vh;
}

.headInfo{
  margin-bottom: 0.1vw;
}

.info{
  margin-bottom: -0.2vw;
  font-family: 'Roboto Slab', 'Times New Roman', Times, serif;
  font-size: 1.1vw;
}

hr {
background-color: #ffffff;
width: 40%;
margin-left: auto;
margin-right: auto;
}

#redot{
  border: 1px solid #f05352;
  border-radius: 50px;
  background-color: #f05352;
  height: 0.75vw;
  width: 0.75vw;
  display: inline-block;

}

.logo {
  height: 5vw;
}


</style>
