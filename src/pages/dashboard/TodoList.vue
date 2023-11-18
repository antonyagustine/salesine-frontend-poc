<template>
  <div class="q-pa-xs" >
    <q-list bordered padding class="q-pa-sm">

      <q-item-label header class="text-bold text-h6">To Do List</q-item-label>

      <q-item-label class="q-pl-md q-pb-sm">Today</q-item-label>

      <q-item clickable tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check1" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Notifications</q-item-label>
          <q-item-label caption>
            Notify me about updates to apps or games that I downloaded
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check2" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Sound</q-item-label>
          <q-item-label caption>
            Auto-update apps at anytime. Data charges may apply
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check3" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Auto-add widgets</q-item-label>
          <q-item-label caption>
            Automatically add home screen widgets
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator spaced />
      <q-item-label header>Yesterday</q-item-label>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check4" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Notifications</q-item-label>
          <q-item-label caption>
            Notify me about updates to apps or games that I downloaded
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check5" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Sound</q-item-label>
          <q-item-label caption>
            Auto-update apps at anytime. Data charges may apply
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check6" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Auto-add widgets</q-item-label>
          <q-item-label caption>
            Automatically add home screen widgets
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator spaced />
      <q-item-label header>Tuesday</q-item-label>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check7" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Notifications</q-item-label>
          <q-item-label caption>
            Notify me about updates to apps or games that I downloaded
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check8" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Sound</q-item-label>
          <q-item-label caption>
            Auto-update apps at anytime. Data charges may apply
          </q-item-label>
        </q-item-section>
      </q-item>

      <q-item tag="label" v-ripple>
        <q-item-section side top>
          <q-checkbox keep-color color="primary" size="xs" dense v-model="check9" />
        </q-item-section>

        <q-item-section>
          <q-item-label>Auto-add widgets</q-item-label>
          <q-item-label caption>
            Automatically add home screen widgets
          </q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'TodoList',
  setup() {
    return {
      check1: ref(false),
      check2: ref(true),
      check3: ref(false),
      check4: ref(true),
      check5: ref(true),
      check6: ref(true),
      check7: ref(true),
      check8: ref(true),
      check9: ref(true)
    }
  }
});
</script>