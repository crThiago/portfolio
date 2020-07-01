<template>
  <nav class="menu d--inline-block bg--white sdw--inset">
    <ul class="d--flex">
      <li class="d--inline">
        <nuxt-link to="/">
          Home
        </nuxt-link>
      </li>
      <li class="d--inline">
        <nuxt-link to="/portfolio">
          Portfólio
        </nuxt-link>
      </li>
      <li class="d--inline">
        <nuxt-link to="/blog">
          Blog
        </nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss">
.menu {
  width: 300px;
  margin-top: 20px;
  padding: 20px 30px;
  border-radius: 50px;

  & ul {
    justify-content: space-between;

    & .active {
      font-weight: bold;
    }
  }
}
</style>
