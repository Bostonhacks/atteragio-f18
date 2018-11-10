<template>
  <div class="Workshops">
    <Live />
    <b-container fluid>
      <b-row id="title">
        <b-col sm="1" />
        <b-col sm="10" md="10">
          <p> Workshops </p>
        </b-col>
      </b-row>
      <b-row>
        <b-col sm="0" md="1" />
        <b-col>
          <Card
            v-for="card in cards"
            :key="card.id"
            :title="card.title"
            :time = "card.time"
            :room = "card.room"
          />
        </b-col>
        <b-col sm="0" md="1" />
      </b-row>
      <Flair />
    </b-container>
  </div>
</template>


<style scoped>

#title{
  margin-top: 10vh;
  font-weight: 300;
  font-size: 3rem;
  padding-bottom: 6vh;
}
</style>

<script>
import Card from "../components/Card.vue"
import Live from "../components/Live.vue"
import Flair from "../components/Flair.vue"

export default {
  name: "Workshops",
  components: {
    Card,
    Live,
    Flair
  },
  data () {
    return {
      cards: [
        {
          title: "Native Smart-Contracts on Bitcoi",
          time: "TBA",
          room: "TBA",
        },
        {
          title: "Intro to HTTP and WebSocket APIs with Bose SoundTouch speakers",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "IBM Cloud Function as the backend for your hackathon app",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to FinTec",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to Git",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to the UR Robot Arm",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Undecided BU AR/VR",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to Backend Development with Node.js and Express",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to Programming for the Robot Operating System (ROS)",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to Web Development with React",
          time: "TBA",
          room: "TBA"
        },
        {
          title: "Intro to Google Cloud Platform",
          time: "TBA",
          room: "TBA"
        }
      ],
    }
  }
}
</script>
