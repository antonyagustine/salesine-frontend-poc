<template>
  <div class="q-pa-md example-row-column-width">
    <div class="row q-pb-md">
      <div class="col text-h4 text-bold	text-primary text-center">
        Dashboard
      </div>
    </div>

    <div class="row q-col-gutter-md">
      <div class="col-4">
        <div class="q-pb-md"><DealsList /></div>
        <div><TodaysHighlight /></div>
      </div>
      <div class="col-4">
        <div><TeamPerformance /></div>
      </div>
      <div class="col-4">
        <div><TodoList /></div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import DealsList from './Deals.vue'
import TodoList from './TodoList.vue'
import TeamPerformance from './TeamPerformance.vue'
import TodaysHighlight from './TodaysHighlight.vue'

export default defineComponent({
  name: 'HomePage',
  components: { DealsList, TodoList, TeamPerformance, TodaysHighlight }
});
</script>
