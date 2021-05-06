<template>
  <div class="circles">
    <div class="circles__circle circles__shape circles_light-red"></div>
    <div class="circles__circle circles__shape circles_dark-blue"></div>
    <div class="circles__circle circles__shape circles_light-yellow"></div>
    <div class="circles__circle circles__shape circles_white"></div>
  </div>
</template>

<script>
export default {
  name: 'ColoredCircles'

}
</script>

<style scoped lang="scss">
@import "../_variables.scss";

.margin-left {
  margin-left: -6vw;

  @media (max-width: 900px) {
    margin-left: -10vh;
  }
}

.circles {
  display: flex;
  position: absolute;

  right: 20vw;
  bottom: 3vh;

  @media (max-width: 900px) {
    right: 6vw;
    bottom: 2vh;
  }

  &__shape {
    border-radius: 50%;
    height: 12vw;
    width: 12vw;

    @media (max-width: 900px) {
      height: 18vh;
      width: 18vh;
    }
  }
  
  &_light-red {
    background-color: $light-red;
  }

  &_dark-blue {
    background-color: $dark-blue;
    @extend .margin-left;
  }

  &_light-yellow {
    background-color: $light-yellow;
    @extend .margin-left;
  }

  &_white {
    background-color: #ffffff;
    @extend .margin-left;
  }
}
</style>