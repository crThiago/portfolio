<template>
  <nuxt-link to="/post" class="card bg--white sdw">
    <div class="card__image">
      <img src="https://picsum.photos/300/200" alt="">
    </div>
    <div class="card__content">
      <Info />
      <h2 class="card__title font--h3 text--justify font--bold color--secondary">
        JavaScript Best Practices for Readable and Maintainable Cod
      </h2>
    </div>
  </nuxt-link>
</template>

<style lang="scss" scoped>
.card {
  transition: scale 1s, box-shadow 1s;

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

  &:hover {
    scale: 1.1;
    box-shadow: 0 0 14px #33333334;
  }
}
</style>
