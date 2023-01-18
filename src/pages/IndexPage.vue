<template>
  <q-page class="row items-center justify-evenly">

    <q-grid class="flex-center" style="overflow: hidden">
      <q-col class="text-center ssCard">
        <img src="/images/clonehero.png" class="ssImg grow" alt="image1"
          @click="clicky('https://clonehero.scorespy.online')">
        <span class="logo">CLONEHERO</span>
      </q-col>
      <q-col class="text-center ssCard">
        <img src="/images/ghtv.png" class="ssImg grow" alt="image2" @click="clicky('https://ghtv.scorespy.online')">
        <span class="logo">GHTV-R</span>
      </q-col>
      <q-col class="text-center ssCard">
        <img src="/images/next.png" class="ssImg grow" alt="image3" style="cursor: not-allowed;">
        <span class="logo">NEXT?</span>
      </q-col>
    </q-grid>

  </q-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  components: {},
  methods: {
    clicky(url: string) {
      window.open(url, '_self')
    }
  }
})
</script>

<style>
.flex-center {
  display: flex;
  align-items: center;
  justify-content: center;
}

.ssCard {
  width: 30vw;
  height: auto;
}

.ssImg {
  width: 30vw;
  height: auto;
  background-size: contain;
  padding: 24px;
  filter: grayscale(90%);
  cursor: pointer;
}

.grow {
  transition: all .2s ease-in-out;
}

.grow:hover {
  transform: scale(1.1);
  filter: grayscale(0%);
}
</style>
