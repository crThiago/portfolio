<template>
  <div class="card bg--white sdw">
    <div class="card__image">
      <img src="https://picsum.photos/300/200" alt="">
    </div>
    <div class="card__content">
      <h2 class="card__title font--h3 text--center font--bold color--secondary">
        {{ project.name }}
      </h2>
      <div class="justify--space-between">
        <span class="font--small">
          Empresa
          <a href="" class="font--bold color--primary">
            {{ project.company.name }}
          </a>
        </span>
        <span class="font--small">
          {{ project.date.start }} - {{ project.date.end }}
        </span>
      </div>
      <p class="card__tech-title font--small text--center">
        Tech
      </p>
      <div class="card__techs justify--space-around">
        <img v-for="tech of project.techs" :key="tech" :src="'/_nuxt/assets/images/' + tech + '.svg'" :alt="tech">
        <!-- <a href=""><img src="~/assets/images/laravel.svg" alt=""></a>
        <a href=""><img src="~/assets/images/php.svg" alt=""></a>
        <a href=""><img src="~/assets/images/graphql.svg" alt=""></a> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    project: {
      type: Object,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.card {
  &__title {
    margin: 10px 0 20px ;
  }

  &__tech-title {
    margin-top: 23px;
    position: relative;

    &::before {
      content: " ";
      width: 40%;
      height: 2px;
      background: #757575;
      position: absolute;
      left: 0;
      top: 5px;
    }
    &::after {
      content: " ";
      width: 40%;
      height: 2px;
      background: #757575;
      position: absolute;
      right: 0;
      top: 5px;
    }
  }

  &__techs {
    padding: 15px 0 30px;

    & img {
      width: 34px;
    }
  }
}
</style>
