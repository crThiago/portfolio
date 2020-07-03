<template>
  <div class="container">
    <Header />
    <main class="blog">
      <h1 class="title-page">
        Blog
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
