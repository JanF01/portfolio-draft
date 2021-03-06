<template>
  <div id="leftmenu">
    <ul>
      <li>PROJECTS <img src="../assets/left-arrow2.png" /></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "LeftMenu",

  methods: {},
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
#leftmenu {
  ul {
    user-select: none;
    list-style-type: none;
    position: absolute;
    bottom: 20%;
    left: 11.4em;
    margin: 0;
    padding: 0;
    color: white;
    li {
      position: relative;
      border: white solid 0.2em;
      font-size: 1.6em;
      font-weight: bold;
      width: 5.5em;
      height: 5.3em;
      letter-spacing: 0.05em;
      border-bottom-left-radius: 2rem;
      transition: 0.2s all;
      &:hover {
        background: rgba(255, 255, 255, 0.18);
        cursor: pointer;
        img {
          bottom: -1.9em;
          left: -1.9em;
        }
      }
      @include flex-center;
      img {
        position: absolute;
        bottom: -1.3em;
        left: -1.3em;
        width: 50%;
        transition: all 0.2s;
      }
    }
  }
}
</style>
