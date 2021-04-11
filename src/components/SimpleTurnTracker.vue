<template>
  <div id="root">
    <div>
      <label>
        Add Player:
        <input>
      </label>
    </div>
  </div>
</template>

<script lang="ts">
import {Component, Vue} from 'vue-property-decorator';

@Component
export default class SimpleTurnTracker extends Vue {
}
</script>

<style scoped>
#root {
  display: flex;
  flex-direction: column;
}
</style>
