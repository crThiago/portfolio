<template>
  <div class="header d--flex">
    <Menu />
    <Social />
  </div>
</template>

<style lang="scss" scoped>
.header {
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap-reverse;
  height: 100px;
}

@media (max-width: 480px) {
  .header {
    justify-content: center;
    height: 145px;
  }
}
</style>
