<template>
  <div class="q-pa-sm" style="background-color: #171717">
    <q-list style="margin-top:40px">
      <PlayerItem v-for="(n, idx) in 10" :key="idx" />
    </q-list>
  </div>
</template>

<script>
import PlayerItem from "../components/PlayerItem";
export default {
  name: "PageIndex",
  components: {
    PlayerItem
  }
};
</script>
