<template>
  <div class="container">
    <div class="text-bar">
      <div class="title">
        <p>Festival</p>
      </div>

      <div class="subtitle">
         We had limited time available here so the quality is not reflective of the potential output.
         <br>
        This capture highlights the main hub of the event with the start and finish lines, and some obstacles. The annotation provides the ability to create an interactive and informative 3D map.  There is a potential opportunity for one of our team members to capture the space the day prior to the event opening and have this model live for race day.
As you can see Festival is not 100% set up for race day yet. We wanted to capture Festival without people around, so we scanned early Friday morning while staff was meeting at basecamp.

      </div>
    </div>

    <div class="content">
      <iframe
      class="frame"
        src="https://sketchfab.com/models/dff58d902d744444895f42f3a11e2851/embed"
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
export default class MainArea extends Vue {}
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
    }
  }
  .subtitle {
    flex: 1;
    margin: 10px;
    font-family: "Montserrat";
    font-size: 12pt;
    text-align: right;
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
