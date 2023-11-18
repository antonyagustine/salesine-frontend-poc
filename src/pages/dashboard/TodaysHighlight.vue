<template>
  <q-list bordered class="rounded-borders q-pa-md">
    <q-item-label header class="text-bold">Today's Highlight</q-item-label>

    <q-item clickable v-ripple>
      <q-item-section>
        <q-item-label class="text-primary" lines="1">Brunch this weekend?</q-item-label>
        <q-item-label caption lines="2">
          <span class="text-weight-bold">Janet</span>
        </q-item-label>
      </q-item-section>

      <q-item-section side top>
        1 min ago
      </q-item-section>
    </q-item>

    <q-separator spaced inset />

    <q-item clickable v-ripple>
      <q-item-section>
        <q-item-label class="text-primary" lines="1">Linear Project</q-item-label>
        <q-item-label caption lines="2">
          <span class="text-weight-bold">John</span>
          -- Can we schedule a call for tomorrow?
        </q-item-label>
      </q-item-section>

      <q-item-section side top>
        30 min ago
      </q-item-section>
    </q-item>

    <q-separator spaced inset />

    <q-item clickable v-ripple>
      <q-item-section>
        <q-item-label class="text-primary" lines="1">Linear Project</q-item-label>
        <q-item-label caption lines="2">
          <span class="text-weight-bold">John</span>
          -- Can we schedule a call for tomorrow?
        </q-item-label>
      </q-item-section>

      <q-item-section side top>
        1 hour ago
      </q-item-section>
    </q-item>

    <q-separator spaced inset />

    <q-item clickable v-ripple>
      <q-item-section>
        <q-item-label class="text-primary" lines="1">Linear Project</q-item-label>
        <q-item-label caption lines="2">
          <span class="text-weight-bold">John</span>
          -- Can we schedule a call for tomorrow?
        </q-item-label>
      </q-item-section>

      <q-item-section side top>
        1 hour ago
      </q-item-section>
    </q-item>
  </q-list>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'TodaysHighlight',
});
</script>