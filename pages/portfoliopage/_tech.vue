<template>
  <div class="container">
    <Header />
    <main class="portfolio">
      <h1 class="title-page">
        {{ title }}
      </h1>
      <div>
        <FilterComponent :techs="techs" />
      </div>
      <div class="portfolio__cards justify--space-around flex--wrap">
        <CardPortfolio v-for="project of projectsFilter" :key="project.slug" :project="project" />
      </div>
    </main>
  </div>
</template>

<script>
import Projects from '~/assets/js/data/projects.js'
import Techs from '~/assets/js/data/techs.js'

export default {
  data () {
    return {
      title: 'Portfólio',
      projects: Projects,
      techs: Techs,
      tech: this.$route.params.tech
    }
  },
  computed: {
    projectsFilter () {
      if (this.tech) {
        return this.projects.filter(p => p.techs.find(t => this.tech === t))
      } else {
        return this.projects
      }
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
