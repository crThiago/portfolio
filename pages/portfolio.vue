<template>
  <div class="container">
    <Header />
    <main class="portfolio">
      <h1 class="portfolio__title text--center font--h1 font--bold color--white">
        Portfólio
      </h1>
      <div class="portfolio__filter">
        <div>
          Filter
        </div>
      </div>
      <div class="portfolio__cards justify--space-between flex--wrap">
        <CardPortfolio />
        <CardPortfolio />
        <CardPortfolio />
      </div>
    </main>
  </div>
</template>

<style lang="scss" scoped>
.portfolio {
  &__title {
    margin: 140px 0 75px;
  }
  &__filter {
    display: inline-block;
    width: 200px;
    height: 200px;
    margin: 60px 60px 60px 0;
    perspective: 600px;

    & > div {
      width: 200px;
      height: 75px;
      background: rgba(255, 0, 0, 0.7);
      line-height: 200px;
      color: white;
      font-size: 18px;
      text-align: center;
      transform: rotateX(59deg);
    }
  }
}
</style>
