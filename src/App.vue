<template>
  <div id="app">
    <main class="content">
      <h1 class="text--center">Simple Turn Tracker</h1>
      <SlamTableCalculator/>
    </main>
  </div>
</template>

<script lang="ts">
import {Component, Vue} from 'vue-property-decorator';
import SimpleTurnTracker from "@/components/SimpleTurnTracker.vue";

@Component({
  components: {
    SlamTableCalculator: SimpleTurnTracker,
  },
})
export default class App extends Vue {
}
</script>

<style>
html, body {
  height: 100vh;
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  height: 100vh;
}

.content {
  flex: 1;
  overflow: auto;
  margin: 40px 60px 0 60px;
}

footer {
  text-align: left;
  padding: 0 8px 5px 8px;
}
</style>
