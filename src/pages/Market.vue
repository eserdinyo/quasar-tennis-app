<template>
  <div class="q-pa-sm" style="background-color: #171717; min-height: 100vh">
    <q-list style="margin-top:40px">
      <MarketItem v-for="(item, idx) in items" :key="idx" :item="item" />
    </q-list>
  </div>
</template>

<script>
import MarketItem from "../components/MarketItem";
export default {
  name: "Market",
  data() {
    return {
      items: [
        {
          id: 1,
          name: "Head Radical Pirate 60 - Küçük Tenis Raketi",
          location: "Istanbul",
          img: require("../assets/images/market/1.png"),
          price: 350
        },
        {
          id: 2,
          name: "Yonex Vcore Pro 97 (310)",
          location: "Ankara",
          img: require("../assets/images/market/2.png"),
          price: 800
        },
        {
          id: 3,
          name: "Az kullanılmış yetişkin tenis raketi",
          location: "Izmir",
          img: require("../assets/images/market/3.png"),
          price: 90
        },
        {
          id: 4,
          name: "wilson pro staff 97 L",
          location: "Antalya",
          img: require("../assets/images/market/4.png"),
          price: 1700
        },
        {
          id: 5,
          name: "Wilson blade 98",
          location: "Bursa",
          img: require("../assets/images/market/5.png"),
          price: 450
        }
      ]
    };
  },
  components: {
    MarketItem
  }
};
</script>
