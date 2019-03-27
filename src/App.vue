<template>
  <div id="app">
    <Navigation></Navigation>
    <PromoVideo></PromoVideo>
    <MainArea></MainArea>
    <SpearMan></SpearMan>
    <ZWalls></ZWalls>
    <SlipWalls></SlipWalls>
    <MonkeyBars></MonkeyBars>
    <StairwayToSparta></StairwayToSparta>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Navigation from '@/components/Navigation.vue';
import PromoVideo from '@/components/PromoVideo.vue';
import ZWalls from '@/components/ZWalls.vue';
import SpearMan from '@/components/SpearMan.vue';
import MonkeyBars from '@/components/MonkeyBars.vue';
import StairwayToSparta from '@/components/StairwayToSparta.vue';
import SlipWalls from '@/components/SlipWalls.vue';
import MainArea from '@/components/MainArea.vue';

@Component({
  components: {
    Navigation,
    PromoVideo,
    SpearMan,
    MonkeyBars,
    ZWalls,
    StairwayToSparta,
    SlipWalls,
    MainArea,
  }
})
export default class App extends Vue {}
</script>

<style>
</style>
