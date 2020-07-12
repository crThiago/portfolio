<template>
  <nav class="menu d--inline-block bg--white sdw--inset">
    <ul class="d--flex">
      <li class="d--inline">
        <nuxt-link class="link" to="/">
          Home
        </nuxt-link>
      </li>
      <li class="d--inline">
        <nuxt-link class="link" to="/portfoliopage">
          Portfólio
        </nuxt-link>
      </li>
      <!-- <li class="d--inline">
        <nuxt-link class="link" to="/blog">
          Blog
        </nuxt-link>
      </li> -->
    </ul>
  </nav>
</template>

<style lang="scss">
.menu {
  width: 200px;
  margin-top: 20px;
  padding: 20px 30px;
  border-radius: 50px;

  & ul {
    justify-content: space-between;
  }
}
.link {
  font-weight: 100;
  transition: font-weight .4s ease-in-out;

  &:hover {
    font-weight: bold;
  }
}

.nuxt-link-exact-active {
  font-weight: bold;
}
</style>
