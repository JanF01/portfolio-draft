<template>
  <div id="rightmenu">
    <ul>
      <li>
        Contact
      </li>
      <li>
        Fiverr
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "RightMenu",

  methods: {},
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
#rightmenu {
  ul {
    user-select: none;
    list-style-type: none;
    position: absolute;
    display: flex;
    top: 4%;
    right: 1.8em;
    border-bottom: white solid 0.25em;
    margin: 0;
    padding: 0;
    padding-right: 10%;
    color: white;
    li {
      font-size: 1.3em;
      height: 2.5rem;
      width: 7.2rem;
      text-align: center;

      @include flex-center;

      transition: all 0.15s;
      &:hover {
        background: $light_blue;
      }
      &:first-child {
        border-top: white solid 0.2em;
        border-left: white solid 0.2em;
        border-right: white solid 0.2em;
      }
      &:nth-child(2) {
        padding-top: 0.2em;
      }
      cursor: pointer;
    }
  }
}
</style>
