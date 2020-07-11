<template>
  <div class="filter">
    <div class="filter__techs justify--center">
      <a class="tech" href="">
        <img class="tech__image" src="~/assets/images/techs/laravel.svg" alt="">
        <span class="tech__name color--white font--bold">Laravel</span>
      </a>
      <a class="tech" href="">
        <img class="tech__image" src="~/assets/images/techs/php.svg" alt="">
        <span class="tech__name color--white font--bold">PHP</span>
      </a>
      <a class="tech" href="">
        <img class="tech__image" src="~/assets/images/techs/graphql.svg" alt="">
        <span class="tech__name color--white font--bold">GraphQL</span>
      </a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.filter {
  max-width: 320px;
  margin: 60px auto;

  &__techs {
    height: 100px;
    background: url('~assets/images/filter-bar.svg') bottom no-repeat;
    background-size: contain;
    align-items: end;
  }
}
.tech {
  padding: 0 10px 15px;
  transition: all .3s;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &__image {
    width: 35px;
  }

  &__name {
    height: 0px;
    display: none;
    font-size: 0.7em;
  }

  &:hover {
    padding: 0 20px 15px;
    margin-bottom: 15px;
    scale: 1.5;

    .tech__name {
      display: block;
    }
  }
}
</style>
