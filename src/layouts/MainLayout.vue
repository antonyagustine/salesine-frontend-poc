<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-avatar style="width: auto;border-radius: unset" class="q-pr-xl">
          <img id="logo" src="~assets/logo.png" alt="logo" style="border-radius: unset">
        </q-avatar>

        <q-tabs
          v-model="tab"
          dense
        >
          <q-tab name="mails" label="Home" />
          <q-tab name="alarms" label="Calls" />
          <q-tab name="deals" label="Deals" />
          <q-tab name="team" label="Team" />
          <q-tab name="activity" label="Activity" />
          <q-tab name="library" label="Library" />
        </q-tabs>

        <q-space />

        <q-input rounded outlined dense v-model="search" label="Search" color="white" class="global-search q-pr-md" input-style="height: 20px">
          <template v-slot:append>
            <q-icon name="search" />
          </template>
        </q-input>

        <div class="q-pr-sm" style="font-weight: bold;">MY ACCOUNT</div>

        <q-btn class="q-pr-sm" flat round dense icon="help" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'MainLayout',
  setup() {
    const search = ref(null)

    return { search, tab: ref('mails') }
  }
});
</script>

<style>
.global-search .q-field__control {
  border: 1px solid white;
}
.global-search .q-field__append, .global-search .q-field__label {
  color: white;
}
</style>
<!-- <style lang="sass" scoped>
#logo {
  width: 174px;
  height: 46px;
  top: 11px;
  left: 10px;
}
</style> -->