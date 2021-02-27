<template>
  <div id="leftmenu">
    <ul>
      <li>
        Projects
      </li>
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
  name: "LeftMenu",

  methods: {},
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
#leftmenu {
  ul {
    list-style-type: none;
    position: absolute;
    bottom: 5%;
    left: 2%;
    color: white;
    li {
      font-size: 1.6em;
      height: 2.5rem;
      width: 7.2rem;
      text-align: center;
      @include flex-center;
      &:hover {
        background: $blue;
        cursor: pointer;
      }
    }
  }
}
</style>
