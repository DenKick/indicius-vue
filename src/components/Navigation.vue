<template>
  <nav class="nav">
    <div class="wrapper wrapper-color">
      <div class="nav__container">
        <div class="nav__logo">
          <a href="/"><img alt="Logo" src="../assets/Logo.png"></a>
        </div>
        <div class="nav__links">
          <ul>
            <li><a href="/">Work</a></li>
            <li><a href="/">Services</a></li>
            <li><a href="/">About</a></li>
            <li><a href="/">Contact</a></li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
}
</script>

<style scoped lang="scss">
@import "../_variables.scss";

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #ffffff;
  font-size: 20px;
  text-decoration: none;
}

.wrapper-color {
  background-color: $light-blue;
}

.nav {
  &__container {
    display: flex;
    font-family: 'Inter', sans-serif;
    height: 80px;
    justify-content: space-between;
  }

  &__logo, &__links {
    align-items: center;
    display: flex;
  }
}
</style>
