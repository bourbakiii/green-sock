<template>
  <div>
    <div class="block green"></div>
    <div class="block black"></div>
  </div>
</template>

<script>
export default {
  mounted() {
    this.$gsap.to(document.querySelector('.green'), { ease:'bounce', x: 1000, duration: 5, marginBottom: 10,})
    this.$gsap.to(document.querySelector('.black'), { ease:'bounce', x: 1000, duration: 5})

  },
}
</script>
<style lang="scss" scoped>
.block {
  width: 100px;
  height: 100px;
  border-radius: 10px;

  &.green {
    background-color: green;
  }

  &.black {
    background-color: black;
  }
}
</style>
