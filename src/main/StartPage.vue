<template>
  <div id="start">
    <main>
      <span> Jan Fiołka - Design And Development </span>
      <StickyNote type="1" class="Sticky-1" draggable="false"></StickyNote>
      <StickyNote type="2" class="Sticky-2" draggable="false"></StickyNote>
    </main>
    <RightMenu></RightMenu>
    <LeftMenu></LeftMenu>
    <DecorationBlock></DecorationBlock>
  </div>
</template>

<script>
import StickyNote from "./StickyNote";
import RightMenu from "./RightMenu";
import LeftMenu from "./LeftMenu";
import DecorationBlock from "./DecorationBlock";
export default {
  name: "StartPage",

  methods: {},
  components: {
    StickyNote,
    RightMenu,
    DecorationBlock,
    LeftMenu,
  },
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
#start {
  animation: bck 4s infinite;
  min-width: 100%;
  height: 100vh;
  background: $dark_blue;
}
main {
  user-select: none;
  background: radial-gradient($dark_blue 30%, transparent);
  min-width: 100%;
  height: 100%;

  color: white;
  font-family: "Barlow Condensed", sans-serif;
  font-size: 1.6em;
  letter-spacing: 0.02em;
  display: flex;
  flex-direction: column;
  align-items: center;
  @include flex-center;
  .Sticky-1 {
    width: 20%;
    transform: rotate(-14deg);
    position: absolute;
    bottom: 10%;
    right: 9%;
    z-index: 1;
  }
  .Sticky-2 {
    width: 18%;
    transform: rotate(20deg);
    position: absolute;
    filter: hue-rotate(-10deg) brightness(90%);
    top: 11%;
    left: 18%;
    z-index: 1;
  }
}
</style>
