<template>
  <div class="container">
    <div class="text-bar">
      <div class="title">
        <p>Z Walls</p>
      </div>

      <div class="subtitle">
An example of a smaller obstacle using the same capture technique.

      </div>
    </div>

    <div class="content">
      <iframe
      class="frame"
        src="https://sketchfab.com/models/740723b1116647cc999b11f8ff1c230c/embed"
        frameborder="0"
        allow="autoplay; fullscreen; vr"
        mozallowfullscreen="true"
        webkitallowfullscreen="true"
      ></iframe>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class ZWalls extends Vue {}
</script>

<style lang="scss" scoped>
// * {
//     color:                    hsla(210, 100%, 100%, 0.9) !important;
//     background:               hsla(210, 100%,  50%, 0.5) !important;
//     outline:    solid 0.25rem hsla(210, 100%, 100%, 0.5) !important;
// }

.container {
  margin: 10px;
  display: flex;
}

.text-bar {
  margin: 10px;
  flex: 1 1 200px;
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  .title {
    flex: 1;
    display: flex;
    flex-direction: column-reverse;
    align-content: flex-end;
    p {
      margin: 10px;
      font-family: "Overpass";
      font-size: 18pt;
      text-align: end;
      text-align: moz-end;
    }
  }
  .subtitle {
    flex: 1;
    margin: 10px;
    font-family: "Montserrat";
    font-size: 12pt;
    text-align: right;
    text-align: moz-right;
  }
}

.content {
  flex: 3 1 auto;
  position: relative;
  overflow: hidden;
  padding-top: 56.25%;
}

.frame {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}

@media all and (max-width: 1040px) {
  .container {
    flex-direction: column-reverse;
  }

  .text-bar {
    flex-direction: row;
    .title {
      flex: 1;
      flex-direction: column;
      align-content: flex-start;
    }
    .subtitle {
      text-align: left;
      flex: 1;
    }
  }
}
</style>
