<template>
  <div class="info justify--space-between">
    <span class="font--small">
      June 17
    </span>
    <span class="info__techs justify--space-around flex--wrap">
      <a href=""><img src="~/assets/images/techs/laravel.svg" alt=""></a>
      <a href=""><img src="~/assets/images/techs/php.svg" alt=""></a>
      <a href=""><img src="~/assets/images/techs/graphql.svg" alt=""></a>
    </span>
  </div>
</template>

<style lang="scss">
.info {
  margin: 10px 0;
  align-items: center;

  &__techs {
    width: auto;

    & img {
      margin: 0 10px;
      width: 22px;
    }
  }
}
</style>
