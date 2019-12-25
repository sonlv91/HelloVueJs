<template>
  <div id="app">
    <div class="wrapper clearfix">
      <players v-bind:scorePlayer="scorePlayer" />

      <controls />

      <dices />

      <input type="number" placeholder="Final score" class="final-score" />
    </div>
  </div>
</template>

<script>
import Players from "./components/Players";
import Controls from "./components/Controls";
import Dices from "./components/Dices";
export default {
  name: "app",
  data() {
    return {};
  },
  components: {
    Players,
    Controls,
    Dices
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
