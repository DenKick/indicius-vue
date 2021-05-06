<template>
  <div class="heading">
    <span :style="style" class="heading__text">{{ text }}</span>
  </div>
</template>

<script>
export default {
  name: 'Heading',
  props: {
    text: String,
    color: String,
    size: String,
    width: String,
  },
  computed: {
    style() {
      return `color: ${this.color};`
    }
  }
}
</script>

<style scoped lang="scss">
.heading__text {
  display: inline-block;
  font-size: 3.3em;
  line-height: 67px;
  width: 550px;

  @media (max-width: 900px) {
    font-size: 2em;
    line-height: 1.5em;
    width: 90%;
  }

  @media (max-width: 400px) {
    font-size: 1.5em;
  }
}
</style>