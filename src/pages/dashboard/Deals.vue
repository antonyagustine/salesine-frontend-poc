<template>
  <div class="row q-col-gutter-md">
    <div class="col-4">
      <q-card flat bordered class="deal-card">
        <q-card-section>
          <div class="text-center q-pb-sm">Total Deals</div>
          <div class="text-h3 text-bold text-center">150</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-4">
      <q-card flat bordered class="deal-card">
        <q-card-section>
          <div class="text-center q-pb-sm">Closed Deals</div>
          <div class="text-h3 text-bold text-center">90</div>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-4">
      <q-card flat bordered class="deal-card">
        <q-card-section>
          <div class="text-center q-pb-sm">Active Deals</div>
          <div class="text-h3 text-bold text-center">60</div>
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'DealsList'
});
</script>

<style lang="scss" scoped>
.deal-card {
  border: 1px solid $primary
}
</style>