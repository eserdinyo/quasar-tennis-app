<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer bordered class="main-nav">
      <q-tabs
        no-caps
        active-color="white"
        indicator-color="transparent"
        class="text-grey"
        v-model="tab"
      >
        <q-route-tab to="/" name="partners" label="Partner Bul" icon="home" />
        <q-route-tab
          to="/courts"
          name="courts"
          label="Kortlar"
          icon="sports_tennis"
        />
        <q-route-tab
          to="/market"
          name="market"
          label="Market"
          icon="storefront"
        />
        <q-route-tab to="/" name="profil" label="Profil" icon="person" />
      </q-tabs>
    </q-footer>
  </q-layout>
</template>

<script>
import { AddressbarColor } from "quasar";
export default {
  name: "MainLayout",
  data() {
    return {
      tab: "partners"
    };
  }
};
</script>
<style lang="scss" scoped>
.main-nav {
  background-color: #303235;
  color: #fff;
}
</style>
