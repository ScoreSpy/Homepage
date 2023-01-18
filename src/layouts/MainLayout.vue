<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-toolbar-title class="logo">
          ScoreSpy
        </q-toolbar-title>

      </q-toolbar>
      <div style="background-color: aqua; width: 100%; height: 4px" class="css-selector" />
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainLayout'
})
</script>

<style>
.css-selector {
    background: linear-gradient(140deg, #ff0000, #fffa00, #18ff00, #00ffeb, #0049ff, #fd00ff, #ff0085);
    background-size: 100% 100%;
}

.logo {
  font-family: 'Spy Agency Bold';
  font-size: xx-large !important
}
</style>
