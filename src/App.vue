<template>
  <router-view />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Dark } from 'quasar'
import './assets/font/Spy_Agency_Bold/stylesheet.css'

export default defineComponent({
  name: 'App',
  setup () {
    Dark.set(true)
  }
})
</script>
