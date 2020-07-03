<template>
  <div class="card bg--white sdw">
    <div class="card__image">
      <img src="https://picsum.photos/300/200" alt="">
    </div>
    <div class="card__content">
      <h2 class="card__title font--h3 text--center font--bold color--secondary">
        Sistema ERP
      </h2>
      <div class="justify--space-between">
        <span class="font--small">
          Empresa
          <a href="" class="font--bold color--primary">
            Mídia Interativa
          </a>
        </span>
        <span class="font--small">
          2017 - Atual
        </span>
      </div>
      <p class="card__tech-title font--small text--center">
        Tech
      </p>
      <div class="card__techs justify--space-around">
        <a href=""><img src="~/assets/images/laravel.svg" alt=""></a>
        <a href=""><img src="~/assets/images/php.svg" alt=""></a>
        <a href=""><img src="~/assets/images/graphql.svg" alt=""></a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  border-radius: 5px;
  overflow: hidden;

  &__content {
    padding: 0 10px;
  }

  &__image > img {
    width: 100%;
  }

  &__title {
    margin: 10px 0 20px ;
  }

  &__tech-title {
    margin-top: 23px;
    position: relative;

    &::before {
      content: " ";
      width: 40%;
      height: 2px;
      background: #757575;
      position: absolute;
      left: 0;
      top: 5px;
    }
    &::after {
      content: " ";
      width: 40%;
      height: 2px;
      background: #757575;
      position: absolute;
      right: 0;
      top: 5px;
    }
  }

  &__techs {
    padding: 15px 0 30px;

    & img {
      width: 34px;
    }
  }
}
</style>
