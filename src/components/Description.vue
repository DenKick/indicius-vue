<template>
  <div class="wrapper">
    <section class="description">
      <div class="description__text">
        <span>We’re a team of humans with the strategy, tools, and talent to build outstanding branding solutions and digital products.</span>
      </div>
      <div class="description__icons">
        
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Description'
}
</script>

<style lang="scss" scoped>
.description {
  background-color: #fff;
  display: grid;
  grid-template-columns: 50% 50%;
  padding: 25vh 0;

  &__text {
    color: #05051E;
    font-size: 2.5em;
  }
;
}
</style>