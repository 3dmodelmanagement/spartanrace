<template>
  <div class="container">
    <div class="logo">
      <div>
        <p>OBSTACLE 3D MODELS</p>
      </div>
    </div>
    <div class="links">
      <div class="link">
Note: The content below is formatted for computer or tablet use, for future work we can optimize for mobile usage. Every scene below the video is interactive and can be navigated with mouse or touchpad
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Navigation extends Vue {
  public data() {
    return {};
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// * {
//     color:                    hsla(210, 100%, 100%, 0.9) !important;
//     background:               hsla(210, 100%,  50%, 0.5) !important;
//     outline:    solid 0.25rem hsla(210, 100%, 100%, 0.5) !important;
// }

.container{
  margin: 10px;
  display: flex;
  flex-wrap: wrap;
}


.logo {
  flex: 1 1 200px;
  font-family: "Overpass Mono";
  padding-top: 40px;
  font-size: 2em;
  display: flex;
  flex-direction: column;
  p {
    margin: 0;
    align-self: flex-end;
    text-align: start;
  }
}

.links {
  flex: 3 1 auto;
  font-family: "Overpass";
  font-size: 1.2em;
  display: flex;
  text-align: start;
  flex-direction: row;
  flex-wrap: wrap;
  align-content: flex-end;
}

.link {
  flex: 1 .33 200px;
}


</style>
