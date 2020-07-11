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
        <CardPortfolio v-for="project of projects" :key="project.slug" :project="project" />
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Portfólio',
      projects: [
        {
          slug: 'sistema-jueri',
          name: 'Sistema Jueri',
          resume: 'Novas Implementações e Criação da versão 3.0',
          link: 'https://www.jueri.com.br',
          company: {
            name: 'Mídia Interativa',
            link: 'https://www.midiainterativa.com.br'
          },
          date: {
            start: '2017',
            end: 'Atual'
          },
          techs: ['css', 'jquery', 'php']
        },
        {
          slug: 'ecommerce-esinstrumentos',
          name: 'ES Instrumentos Musicais',
          resume: 'Criação de e-commerce',
          link: 'https://www.esinstrumentosmusicais.com.br/',
          company: {
            name: 'Mídia Interativa',
            link: 'https://www.midiainterativa.com.br'
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['bootstrap', 'workcontrol', 'rest']
        },
        {
          slug: 'sistema-uninova',
          name: 'Uninova Saúde',
          resume: 'Criação de sistema de cadastro, agendamento de consultas, histórico de consultas, controle de financeiro e mais...',
          link: 'https://uninovasaude.com.br/',
          company: {
            name: 'Rem Soft',
            link: 'https://www.remsoft.com.br/'
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['php', 'css', 'jquery']
        },
        {
          slug: 'sistema-petra',
          name: 'Petra Gestão',
          resume: 'Criação de sistema de workflow para contratação de novos colaboradores para as empresas parceiras',
          link: 'https://www.petracorporate.com.br/',
          company: {
            name: '',
            link: ''
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['php', 'css', 'jquery']
        },
        {
          slug: 'sistema-sintras',
          name: 'Sintras',
          resume: 'Novas implementações no sistema de agendamento de consultas',
          link: 'http://www.sintras.net/',
          company: {
            name: 'Mídia Interativa',
            link: 'https://www.midiainterativa.com.br'
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['php', 'css', 'jquery']
        },
        {
          slug: 'casasanta',
          name: 'Casasanta Alimentos',
          resume: 'Criação de site',
          link: 'http://casasantaalimentos.com.br/',
          company: {
            name: 'Mídia Interativa',
            link: 'https://www.midiainterativa.com.br'
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['css', 'jquery']
        },
        {
          slug: 'tectapetes',
          name: 'Tectapetes',
          resume: 'Criação de site',
          link: 'http://www.tectapetes.com.br/',
          company: {
            name: 'Mídia Interativa',
            link: 'https://www.midiainterativa.com.br'
          },
          date: {
            start: '',
            end: ''
          },
          techs: ['css', 'jquery']
        }
      ]
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
