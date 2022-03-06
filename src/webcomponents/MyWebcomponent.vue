<template>
  <div>
    <group-card />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

import GroupCard from "@/components/group-card/GroupCard.vue";

@Component({
  components: {
    GroupCard,
  }
})
export default class PncGroupRegistration extends Vue {}
</script>

<style lang="scss">
// This is because I use rem, so to make it behave everywhere the same I set the root font-size
:host {
  font-size: 100px !important;
}
</style>

<style lang="scss">
.app {
  text-align: left;
  max-width: 440px;
}
</style>