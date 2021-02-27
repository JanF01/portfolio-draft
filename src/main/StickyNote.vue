<template>
  <div id="stickynote">
    <header></header>
    <img
      src="../assets/sticky_noteAngular.png"
      v-if="type == 1"
      draggable="false"
    />
    <img
      src="../assets/sticky_noteFoundation.png"
      v-if="type == 2"
      draggable="false"
    />
  </div>
</template>

<script>
export default {
  name: "StickyNote",
  props: {
    type: Number,
  },
  methods: {},
};
</script>

<style scoped lang="scss">
@import "../mixins/mixins.scss";
img {
  width: 100%;
  animation: randomMovement 7s infinite;
}
</style>
