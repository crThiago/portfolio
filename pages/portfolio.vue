<template>
  <div class="container">
    <Header />
    <main class="portfolio">
      <h1 class="portfolio__title text--center font--h1 font--bold color--white">
        Portfólio
      </h1>
      <div>
        <FilterComponent />
      </div>
      <div class="portfolio__cards justify--space-around flex--wrap">
        <CardPortfolio />
        <CardPortfolio />
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
}
</style>
