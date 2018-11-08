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
          title: "Intro to Web dev",
          time: "2:00 - 3:00",
          room: "Room 320",
        },
        {
          title: "Unit 3D",
          time: "2:00 - 3:00",
          room: "Room 228"
        }
      ],
    }
  }
}
</script>
