<template>
  <div>
    <b-container class="bv-example-row">
        <b-row class="homeHead">
            <b-col>Flair</b-col>
            <b-col cols="6" id="heroText">
              <div >
                <p class="heroText"> Boston<span id="bolder">Hacks</span> 2018 </p>
                <p>why is this doing stupid stuff</p>
              </div>
            </b-col>
            <b-col>Flair</b-col>
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
  width: 45vh;
}
.heroText {
  color: white;
  font-family: "Roboto", Arial, Helvetica, sans-serif;
  font-weight: 400;
  font-size: 3.7vw;
  display: inline;
}

#bolder {
  font-weight: 700;
}

.homeHead{
  padding-top: 10vw;
}


</style>
