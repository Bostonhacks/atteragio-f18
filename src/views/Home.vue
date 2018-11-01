<template>
  <div>
    <b-container> 
        <b-row class="homeHead">
            <b-col>Flair</b-col>
            <b-col cols="6" id="heroText">
              <div >
                <p class="heroText"> Boston<span id="bolder">Hacks</span> 2018 </p>
                <p class="date">November 10 &#8211 November 11,2018<br>
                775 Commonwealth Avenue, Boston University</p>
              </div>
            </b-col>
            <b-col>Flair</b-col>
        </b-row>
    </b-container>
    <b-container>
      <b-row>
        <b-col>Wifi</b-col>
        <b-col>Slack</b-col>
        <b-col>Devpost</b-col>
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


#heroText{
}
.heroText {
  color: white;
  font-family: "Roboto", Arial, Helvetica, sans-serif;
  font-weight: 400;
  font-size: 3.7vw;
}

.date{
  margin-top: -1vh;
  line-height: 2vw;
}

#bolder {
  font-weight: 700;
}

.homeHead{
  padding-top: 1vh;
}
@media (max-width: 600px) {
  .homeHead {
    margin-top: -5vw;
  }
}

</style>
