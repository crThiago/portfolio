<template>
  <div class="filter">
    <div class="filter__techs justify--center">
      <nuxt-link v-for="tech of techs" :key="tech.slug" class="tech" :to="`/portfoliopage/${tech.slug}`">
        <img class="tech__image" :src="techimage(tech.slug)">
        <span class="tech__name color--white font--bold">{{ tech.name }}</span>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    techs: {
      required: true,
      type: Array
    }
  },
  methods: {
    techimage: tech => require(`~/assets/images/techs/${tech}.svg`)
  }
}
</script>

<style lang="scss" scoped>
.filter {
  max-width: 320px;
  margin: 60px auto;

  &__techs {
    height: 100px;
    background: url('~assets/images/filter-bar.svg') bottom no-repeat;
    background-size: contain;
    align-items: end;
  }
}
.tech {
  padding: 0 10px 15px;
  transition: all .3s;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &__image {
    width: 35px;
  }

  &__name {
    text-align: center;
    height: 0px;
    display: none;
    font-size: 0.7em;
  }

  &:hover {
    padding: 0 20px 15px;
    margin-bottom: 15px;
    scale: 1.5;

    .tech__name {
      display: block;
    }
  }
}
.nuxt-link-active {
  padding: 0 20px 15px;
  margin-bottom: 15px;
  scale: 1.5;

  .tech__name {
    display: block;
  }
}
</style>
