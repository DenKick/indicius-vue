<template>
  <Header />
</template>

<script>
import Header from './components/Header';

export default {
  name: 'App',
  components: {
    Header
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
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
