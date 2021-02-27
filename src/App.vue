<template>
  <div id="app">
    <StartPage class="start"></StartPage>
  </div>
</template>

<script>
import StartPage from "./main/StartPage.vue";

export default {
  name: "App",
  components: {
    StartPage,
  },
};
</script>

<style>
@import "./mixins/mixins.scss";
body {
  margin: 0 auto;
  overflow-y: hidden;
}
#app {
  width: 100%;
  height: 100%;
  font-family: "Abel", sans-serif;
}
.start {
  width: 100%;
  height: 100%;
}
</style>
