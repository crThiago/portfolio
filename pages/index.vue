<template>
  <div class="container d--flex flex--column">
    <div class="header d--flex">
      <Menu />
      <Social />
    </div>
    <section class="home d--flex">
      <div class="home__description">
        <h1 class="home__description__title font--h1 font--bold color--white">
          Olá, me chamo Thiago
        </h1>
        <h2 class="font--h2 font--bold color--secondary">
          Sou programador FullStack Web, mais especificamente na linguagem PHP
        </h2>
      </div>
      <div class="home__image">
        <img class="d--inline border--secondary" src="https://avatars3.githubusercontent.com/u/33141686?s=460&u=0081b9777c63192214cc88ece924e244a817d090&v=4" alt="">
      </div>
    </section>
  </div>
</template>

<style lang="scss">
.container {
  max-width: 1200px;
  height: 100vh;
  margin: 0 auto;
  padding: 20px;
}
.header {
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap-reverse;
}

@media (max-width: 480px) {
  .header {
    justify-content: center;
    margin: 20px 0;
  }
}

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
    text-align: right;
    & > img {
      width: 75%;
      border-radius: 15px;
      border: 5px solid;
    }
  }
}
@media (max-width: 900px) {
  .container {
    height: auto;
  }

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
