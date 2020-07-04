<template>
  <div class="container">
    <Header />
    <main class="blog">
      <h1 class="title-page">
        {{ title }}
      </h1>
      <div>
        <FilterComponent />
      </div>
      <div class="blog__cards justify--space-around flex--wrap">
        <CardBlog />
        <CardBlog />
        <CardBlog />
        <CardBlog />
        <CardBlog />
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Blog'
    }
  },
  head () {
    return {
      title: 'Dicas valiosas sobre PHP, Laravel, Vue, Nuxt, CSS, SASS - ' + this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content: 'Aprenda junto comigo sobre PHP, Laravel, Vue, Nuxt, CSS, SCSS e outras tecnologias incríveis :D'
        }
      ]
    }
  }
}
</script>
