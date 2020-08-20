<template>
  <div class="q-pa-sm" style="background-color: #171717">
    <q-list style="margin-top:40px">
      <CourtItem v-for="(court, idx) in courts" :key="idx" :court="court" />
    </q-list>
  </div>
</template>

<script>
import CourtItem from "../components/CourtItem";
export default {
  data() {
    return {
      courts: [
        {
          id: 1,
          name: "Moda Sahil Tenis Kortu",
          location: "Kadıköy / Istanbul",
          img: require("../assets/images/courts/1.jpeg")
        },
        {
          id: 2,
          name: "Kartal Belediye Tenis Kortu",
          location: "Kartal / Istanbul",
          img: require("../assets/images/courts/2.jpeg")
        },
        {
          id: 3,
          name: "Pendik Tenis Kortu",
          location: "Pendik / Istanbul",
          img: require("../assets/images/courts/3.jpg")
        },
        {
          id: 4,
          name: "Bebek Sahil Tenis Kortu",
          location: "Beşiktaş / Istanbul",
          img: require("../assets/images/courts/4.jpg")
        },
        {
          id: 5,
          name: "Maltepe Sahil Tenis Kortu",
          location: "Maltepe / Istanbul",
          img: require("../assets/images/courts/5.jpg")
        }
      ]
    };
  },
  components: {
    CourtItem
  }
};
</script>

<style lang="scss" scoped></style>
