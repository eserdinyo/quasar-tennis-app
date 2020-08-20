<template>
  <q-item
    class="CourtItem"
    :style="{
      background: `url('${court.img}')`
    }"
    clickable
    v-ripple
  >
    <div class="CourtItem-footer">
      <q-item-section>
        <q-item-label class="text-white q-mb-xs text-weight-bold">{{
          court.name
        }}</q-item-label>
        <q-item-label class="text-white row">
          <q-icon name="location_on" color="white q-mr-xs" />
          {{ court.location }}</q-item-label
        >
      </q-item-section>
    </div>
  </q-item>
</template>

<script>
export default {
  props: {
    court: {
      type: Object,
      required: true
    }
  }
};
</script>

<style lang="scss" scoped>
.CourtItem {
  padding: 0;
  background-position: center !important;
  background-size: cover !important;
  border-radius: 8px;
  margin-bottom: 10px;
  height: 150px;
  overflow: hidden;

  &-footer {
    background: rgba(0, 0, 0, 0.7);
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    padding: 10px 18px;
  }
}
</style>
