<template>
  <q-card flat bordered class="q-pa-xs">
    <q-card-section>
      <q-item-label header class="text-bold text-h6 q-pa-none">Team performance</q-item-label>
    </q-card-section>
    <q-card-section class="q-pt-xs">
      <Pie :data="chartData" :options="chartOptions" />
    </q-card-section>
  </q-card>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Pie } from 'vue-chartjs'
import { Chart as ChartJS, ArcElement, Tooltip, Legend, ChartOptions } from 'chart.js'

ChartJS.register(ArcElement, Tooltip, Legend)

export default defineComponent({
  name: 'TeamPerformance',
  components: {
    Pie
  },
  setup() {
    const chartData = {
      labels: ['Not so well', 'Extremely well', 'Somewhat well'],
      datasets: [
        {
          backgroundColor: ['#606060', '#E5EFFF', '#3F51B5'],
          data: [15, 64, 25]
        }
      ]
    }

    const chartOptions: ChartOptions = {
      responsive: true,
      plugins: {
        legend: {
          labels: {
            boxWidth: 20,
            boxHeight: 20,
          },
          align: 'end',
          position: 'right'
        }
      },
      maintainAspectRatio: false
    }
    return { chartData, chartOptions }
  }
});
</script>