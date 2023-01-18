<template>
  <q-page class="row items-center justify-evenly">

    <div class="row" style="overflow: hidden">
      <div class="text-center ssCard">
        <img src="/images/clonehero.png" class="ssImg grow" alt="image1"
          @click="clicky('https://clonehero.scorespy.online')">
        <span class="logoFlex">CLONEHERO</span>
      </div>
      <div class="text-center ssCard">
        <img src="/images/ghtv.png" class="ssImg grow" alt="image2" @click="clicky('https://ghtv.scorespy.online')">
        <span class="logoFlex">GHTV-R</span>
      </div>
      <div class="text-center ssCard">
        <img src="/images/next.png" class="ssImg grow" alt="image3" style="cursor: not-allowed;">
        <span class="logoFlex">NEXT?</span>
      </div>
    </div>

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
.logoFlex {
  font-family: 'Spy Agency Bold';
  line-height: 1em;
  max-height: 2em;
  font-size: 3vw;
}

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
