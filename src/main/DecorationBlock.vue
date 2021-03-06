<template>
  <div id="decorationblock">
    <div class="cite">
      IDEAS / DESIGN / DEVELOPMENT
    </div>
    <div class="left-decoration">
      <div class="first-block"></div>
      <div class="second-block"></div>
      <div class="third-block"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DecorationBlock",
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
#decorationblock {
  .cite {
    user-select: none;
    writing-mode: vertical-lr;
    text-orientation: mixed;
    position: absolute;
    right: 1em;
    top: 0;
    height: 100vh;
    text-align: center;
    color: white;
    font-size: 1.4em;
    letter-spacing: 0.17em;
    font-weight: bold;
  }
  .left-decoration {
    position: absolute;
    top: 1.9%;
    left: 0;
    div {
      margin-top: 1em;
      border-bottom-right-radius: 1em;
    }
    .first-block {
      height: 1.2em;
      width: 9em;
      background: white;
    }
    .second-block {
      height: 1.2em;
      width: 7em;
      background: white;
    }
    .third-block {
      height: 1.2em;
      width: 5em;
      background: white;
    }
  }
}
</style>
