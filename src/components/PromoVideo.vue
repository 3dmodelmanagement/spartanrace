<template>
  <div class="container">
    <div class="content">
      <iframe
        class="frame"
        src="https://www.youtube.com/embed/1RWC6hqKDM4"
        frameborder="0"
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="text">
      <p>
        This video shows the potential to highlight the context of each particular course and how the obstacles inhabit the terrain. A video like this could bring you from start to finish, and at each obstacle provide a link with the option to view the associated Obstacle 3D Model.  This video was to spark curiosity and potential in how you can view a location specific course and then connect with something interactive.

         It is also a tool to examine how the existing Spartan Youtube account could be leveraged to connect video with 3D content using Youtube Cards, which appear in the top right corner at different moments throughout the duration.  This is particularly relevant to the Ring The Bell Youtube series.  (The YouTube card links that currently appear on the video connect with other Spartan videos for your example, but we can link to any specific Spartan video or 3D model.)

      </p>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class PromoVideo extends Vue {}
</script>

<style lang="scss" scoped>
// * {
//     color:                    hsla(210, 100%, 100%, 0.9) !important;
//     background:               hsla(210, 100%,  50%, 0.5) !important;
//     outline:    solid 0.25rem hsla(210, 100%, 100%, 0.5) !important;
// }

.container {
  margin: 0px;
}

.content {
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

.text {
    margin: 10px;
    font-family: "Montserrat";
    font-size: 12pt;
}

// @media all and (max-width: 1040px) {
//   .container {
//     flex-direction: column-reverse;
//   }

//   .text-bar {
//     flex-direction: row;
//     .title {
//       flex: 1;
//       flex-direction: column;
//       align-content: flex-start;
//     }
//     .subtitle {
//       text-align: left;
//       flex: 1;
//     }
//   }
// }
</style>
