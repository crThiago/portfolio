<template>
  <div class="card bg--white sdw">
    <div class="card__image">
      <img src="https://picsum.photos/300/200" alt="">
    </div>
    <div class="card__content">
      <div class="card__info justify--space-between">
        <span class="font--small">
          June 17
        </span>
        <span class="card__techs justify--space-around">
          <a href=""><img src="~/assets/images/laravel.svg" alt=""></a>
          <a href=""><img src="~/assets/images/php.svg" alt=""></a>
          <a href=""><img src="~/assets/images/graphql.svg" alt=""></a>
        </span>
      </div>
      <h2 class="card__title font--h3 text--justify font--bold color--secondary">
        JavaScript Best Practices for Readable and Maintainable Code
      </h2>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  &__info {
    margin: 10px 0;
    align-items: center;
  }

  &__techs {
    width: 50%;

    & img {
      width: 22px;
    }
  }

  &__title {
    margin: 10px 0;
  }
}
</style>
