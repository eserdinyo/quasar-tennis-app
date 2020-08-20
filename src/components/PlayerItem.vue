<template>
  <q-item class="PlayerItem" clickable v-ripple>
    <q-item-section avatar>
      <q-avatar>
        <img :src="`https://randomuser.me/api/portraits/women/68.jpg`" />
      </q-avatar>
    </q-item-section>

    <q-item-section>
      <q-item-label class="text-white q-mb-xs text-weight-bold"
        >Alex, 24 Yaşında</q-item-label
      >
      <q-item-label class="text-white row items-center">
        <q-icon name="location_on" color="white q-mr-xs" /> Ankara</q-item-label
      >
    </q-item-section>

    <q-item-section side class="text-white q-mt-xl">
      <b>ITN 5</b>
    </q-item-section>
  </q-item>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.PlayerItem {
  padding: 10px;
  background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
    url("../assets/images/player-bg.jpg");
  background-size: cover;
  border-radius: 8px;
  margin-bottom: 10px;
}

.q-item__section--side > .q-avatar {
  font-size: 80px !important;
}
</style>
