<template>
  <Header />
  <Description />
</template>

<script>
import Header from './components/Header';
import Description from './components/Description';

export default {
  name: 'App',
  components: {
    Header,
    Description
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
}

.wrapper {
  padding: 0 12vw;

  @media (max-width: 900px) {
    padding: 0 6vw;
  }
}

#app {
  font-family: 'DM Sans', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
