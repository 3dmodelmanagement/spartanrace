<template>
  <div class="container">
    <div class="logo">
      <div>
        <p>Spartan</p>
        <p>Race</p>
      </div>
    </div>
    <div class="links">
      <div class="link">
3D Model Management traveled to Diablo Grande,
California to capture the amazing course and setting of the San Jose Super and Sprint Weekend.  
<br>
Our team put together a collection of obstacles from the race and converted them to interactive 3D models as a demonstration of potential content.
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
    text-align: end;
  }
}

.links {
  flex: 3 1 auto;
  font-family: "Overpass";
  font-size: 1.2em;
  margin-left: 20px;
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
