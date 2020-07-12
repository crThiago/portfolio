<template>
  <div class="card bg--white sdw">
    <div class="card__image">
      <img :src="thumbnail" :alt="project.name">
    </div>
    <div class="card__content">
      <h2 class="card__title font--h3 text--center font--bold color--secondary">
        <a :href="project.link" target="_blank" rel="nofollow noopener noreferrer">{{ project.name }}</a>
      </h2>
      <div class="justify--space-between">
        <span class="font--small">
          Empresa
          <a :href="project.company.link" class="font--bold color--primary" target="_blank" rel="nofollow noopener noreferrer">
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
        <nuxt-link v-for="tech of project.techs" :key="tech" :to="`/portfoliopage/${tech}`">
          <img :src="techimage(tech)" :alt="tech">
        </nuxt-link>
      </div>
    </div>
    <span class="card__resume" />
    <p class="resume__text">
      {{ project.resume }}
    </p>
  </div>
</template>

<script>
export default {
  props: {
    project: {
      type: Object,
      required: true
    }
  },
  computed: {
    thumbnail () {
      return require(`~/assets/images/portfolio/${this.project.slug}.jpeg`)
    }
  },
  methods: {
    techimage: tech => require(`~/assets/images/techs/${tech}.svg`)
  }
}
</script>

<style lang="scss" scoped>
.card {
  flex: 1 1 300px;
  position: relative;

  &__resume {
    bottom: 5px;
    left: 5px;
    position: absolute;
    width: 20px;
    height: 20px;
    background: #35495e;
    border-radius: 50px;
    transition: all .3s;
    z-index: 4;

    &:hover, &:active {
      transform: scale(55);
      transition: all .3s;
      &  + .resume__text {
          opacity: 1;
          transition: all 0.4s;
      }
    }
  }

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
.resume__text {
  position: absolute;
  opacity: 0;
  z-index: 5;
  top: 0px;
  padding: 15px;
  font-size: 1.5em;
  line-height: 49px;
  font-weight: bolder;
  color: white;
}
</style>
