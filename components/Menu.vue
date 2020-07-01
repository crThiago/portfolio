<template>
  <nav class="menu d--inline-block bg--white sdw--inset">
    <ul class="d--flex">
      <li class="d--inline">
        <a class="active" href="#">Home</a>
      </li>
      <li class="d--inline">
        <a href="#">Portfolio</a>
      </li>
      <li class="d--inline">
        <a href="#">Blog</a>
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
