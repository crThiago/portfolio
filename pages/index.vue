<template>
  <div class="container">
    <div class="header d--flex">
      <Menu />
      <Social />
    </div>
    <section>
      <div>
        <h1 class="font--h1 font--bold color--white">
          Olá, me chamo Thiago
        </h1>
        <h2 class="font--h2 font--bold color--secondary">
          Sou programador FullStack Web, mais especificamente na linguagem PHP
        </h2>
      </div>
      <div>
        <img src="https://avatars3.githubusercontent.com/u/33141686?s=460&u=0081b9777c63192214cc88ece924e244a817d090&v=4" alt="">
      </div>
    </section>
  </div>
</template>

<style lang="scss">
.container {
  width: 1200px;
  margin: 0 auto;
}
.header {
  justify-content: space-between;
  align-items: center;
}
</style>
