<template>
  <div class="Prizes">
    <Live />
    <b-container fluid>
      <b-row id="title">
        <b-col cols=1 />
        <b-col id="header">
          <p> Challenges & Prizes </p>
        </b-col>
      </b-row>
      <b-row id="infoRow">
        <b-col cols=1 />
        <b-col>
          <p class="category"> Giving Back to Veterans </p>
          <p class="prizeItem"> Amazon Echo Sports </p>
          <p class="info"> Veterans risked their lives to let you sit in the
            comfort of your home, or at BostonHacks, and code. It’s time to give
            back and create solutions for problems countless veterans face every
            day.
          </p>
        </b-col>
        <b-col>
          <p class="category"> The Smart Home </p>
          <p class="prizeItem"> Google Home Hub and 2 Lights Starter Pack </p>
          <p class="info">Learn how to create Internet of Things devices and
            robots to realize the dream of the smart home. Get your hands on
            state-of-the-art hardware and study the intimate interaction of
            humans and technology.
          </p>
        </b-col>
        <b-col>
          <p class="category"> Data for Urban Good </p>
          <p class="prizeItem">Surface Go Tablets, Typecovers, and Surface Pens</p>
          <p class="info"> Your hometown works every day to improve the quality
            of life for its residents. Help out your local city/town by
            utilizing their robust datasets and collecting insights for urban
            improvements.
          </p>
        </b-col>
        <b-col cols=1 />
      </b-row>
      <b-row>
        
      </b-row>

      <Flair />
    </b-container>
  </div>
</template>

<style scoped>
.Prizes {
}

.category {
  margin-top: 4vh;
  font-size: 1.3vw;
}

.info{
  font-weight: 300;
  font-size: 1.1vw;
  margin-top: -2vh;
}
.prizeItem {
  font-size: 1.25vw;
  margin-top: 3vh;
}
#header {
  font-weight: 300;
  font-size: 2vw;
}

#title{
  margin-top: 10vh;
}

#infoRow {
  margin-top: 6vh;
}

#bolder {
  font-weight: 700;
  text-align: center;
}

#redot{
  border: 1px solid #f05352;
  border-radius: 50px;
  background-color: #f05352;
  height: 0.75vw;
  width: 0.75vw;
  display: inline-block;

}

</style>

<script>
  export default {
    name: "Faq",
    components: {
      Live,
      Flair
    }
  };

  import Live from "../components/Live.vue"
  import Flair from "../components/Flair.vue"
</script>
