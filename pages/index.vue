<template>
  <div class="container d--flex flex--column">
    <Header />
    <section class="home d--flex">
      <div class="home__description">
        <h1 class="home__description__title font--h1 font--bold color--white">
          Olá, me chamo Thiago
        </h1>
        <h2 class="font--h2 font--bold color--secondary">
          Sou programador FullStack Web, mais especificamente na linguagem PHP
        </h2>
      </div>
      <div class="home__image text--right">
        <img class="d--inline border--secondary" src="https://avatars3.githubusercontent.com/u/33141686?s=460&u=0081b9777c63192214cc88ece924e244a817d090&v=4" alt="">
      </div>
    </section>
  </div>
</template>

<style lang="scss">
.home {
  flex-grow: 1;
  align-items: center;

  &__description {
    width: 50vw;

    &__title {
      margin: 30px 0;
    }
  }

  &__image {
    width: 50vw;
    & > img {
      width: 55%;
      border-radius: 15px;
      border: 5px solid;
    }
  }
}
@media (max-width: 900px) {
  .home {
    flex-wrap: wrap-reverse;
    text-align: center;

    &__description {
      width: 100vw;
    }

    &__image {
      margin: 20px auto;
      width: auto;

      & > img {
        width: 200px;
      }
    }
  }
}
</style>
