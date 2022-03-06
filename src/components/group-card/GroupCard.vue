<template>
  <div class="group-card">
    <h4 class="title">GROUP NAME</h4>
    <span class="description">Some description</span>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  components: {},
})
export default class GroupCard extends Vue {}
</script>

<style lang="scss" scoped>
.group-card {
  padding: 2rem;
  margin: 2rem;
  background-color: #2a8ada;

  .title {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .description {
      font-size: 1.5rem;
  }
}
</style>