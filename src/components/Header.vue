<template>
  <header class="header">
    <Navigation />
    <div class="wrapper">
      <div class="header__content">
        <Heading text="Designing for a more human-centered world." color="#ffffff" size="3.3em"/>
        <Heading text="Together." color="#FFCC00" size="3.3em"/>
      </div>
    </div>
    <ColoredCircles />
  </header>
</template>

<script>
import Navigation from './Navigation';
import Heading from './Heading';
import ColoredCircles from './ColoredCircles';

export default {
  name: 'Header',
  components: {
    Navigation,
    Heading,
    ColoredCircles,
  }
}
</script>

<style scoped lang="scss">
@import "../_variables.scss";

.header {
  background-color: $light-blue;
  height: 100vh;
  position: relative;

  @media (max-width: 900px) and (orientation: portrait) {
    height: 94vh;
  }

  &__content {
    padding: 20vh 0 0 0;
  }

  &__content {
    height: 100%;
  }
}
</style>