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
