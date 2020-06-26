<template>
  <nav class="menu bg--white shadown--inset">
    <ul>
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
  display: inline-block;
  margin-top: 20px;
  padding: 20px 30px;
  border-radius: 50px;
  background: white;
  box-shadow: inset 0px 0px 4px #33333334;

  & li {
    margin: 0 30px;

    & .active {
      font-weight: bold;
    }
  }
}

.d--inline {
  display: inline
}
</style>
