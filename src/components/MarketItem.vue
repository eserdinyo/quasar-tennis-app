<template>
  <q-item class="MarketItem" clickable v-ripple>
    <q-item-section avatar>
      <q-avatar square>
        <img :src="item.img" />
      </q-avatar>
    </q-item-section>

    <q-item-section>
      <q-item-label class="text-white q-mb-xs">{{ item.name }}</q-item-label>
      <q-item-label class="text-grey row items-center">
        <q-icon name="location_on" color="grey q-mr-xs" />
        {{ item.location }}</q-item-label
      >
    </q-item-section>

    <q-item-section side class="text-white q-mt-xl">
      <h6>{{ item.price }} ₺</h6>
    </q-item-section>
  </q-item>
</template>

<script>
export default {
  props: {
    item: {
      type: Object,
      required: true
    }
  }
};
</script>

<style lang="scss" scoped>
.MarketItem {
  padding: 0;
  background-color: #2a2a2a;
  border-radius: 8px;
  margin-bottom: 10px;
  overflow: hidden;
  height: 100px;
  padding-right: 10px;

  .q-item__section--side > .q-avatar {
    height: 100%;
    width: 100px;
  }
}
</style>
