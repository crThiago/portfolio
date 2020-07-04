<template>
  <div class="filter">
    <div class="justify--center">
      <a href=""><img class="tech__image" src="~/assets/images/laravel.svg" alt=""></a>
      <a href=""><img class="tech__image" src="~/assets/images/php.svg" alt=""></a>
      <a href=""><img class="tech__image" src="~/assets/images/graphql.svg" alt=""></a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.filter {
  max-width: 320px;
  margin: 60px auto;
  background: url('~assets/images/filter-bar.svg') bottom no-repeat;
  background-size: contain;
}

.tech__image {
  width: 35px;
  padding: 0 10px 15px;
  transition: all .3s;

  &:hover {
    scale: 1.5;
    padding: 0 20px 15px;
  }
}
</style>
