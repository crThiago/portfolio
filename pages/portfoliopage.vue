<template>
  <div class="container">
    <Header />
    <main class="portfolio">
      <h1 class="title-page">
        {{ title }}
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

<script>
export default {
  data () {
    return {
      title: 'Portfólio'
    }
  },
  head () {
    return {
      title: 'Experiência na criação de lojas virtuais, e-commerces, sistemas e sites - ' + this.title,
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

<style lang="scss" scoped>
.portfolio {
  &__title {
    margin: 140px 0 75px;
  }
}
</style>
