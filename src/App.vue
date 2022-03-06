<template>
  <div id="app">
    <my-webcomponent />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

import MyWebcomponent from "@/webcomponents/MyWebcomponent.vue";

@Component({
  components: {
    MyWebcomponent,
  },
})
export default class App extends Vue {
}
</script>

<style scoped>
#app {
  margin: 16px;
}
</style>
