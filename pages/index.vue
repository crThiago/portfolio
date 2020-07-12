<template>
  <div class="container h-100 d--flex flex--column">
    <Header />
    <section class="home d--flex">
      <div class="home__description">
        <h1 class="home__description__title font--h1 font--bold color--white">
          Programador <strong>Front-end</strong> & <strong>Back-end</strong>
        </h1>
        <h2 class="home__description__subtitle font--h2 font--bold color--secondary">
          Me chamo Thiago Costa tenho 30 anos e trabalho como desenvolvedor web a 5 anos,
          tenho graduação no curso de Engenharia de Computação pela Unopar de Londrina - PR.
        </h2>
      </div>
      <div class="home__image text--right">
        <img class="d--inline border--secondary" src="https://avatars3.githubusercontent.com/u/33141686?s=460&u=0081b9777c63192214cc88ece924e244a817d090&v=4" alt="">
      </div>
    </section>
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Conheça um pouco sobre mim - programador Front-end e Back-end',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content: `Tenho experiência com a criação de sites, e-commerces / loja Virtuais, sistemas e muito mais, 
          confira meu portólio`
        }
      ]
    }
  }
}
</script>

<style lang="scss">
.home {
  flex-grow: 1;
  align-items: center;

  &__description {
    width: 70vw;

    &__title {
      line-height: 50px;
      margin: 30px 0;
    }

    &__subtitle {
      line-height: 50px
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
