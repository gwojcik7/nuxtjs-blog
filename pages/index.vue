<template>
  <Container class="home grid">
    <Hero>
      <template v-slot:heading>Cześć!</template>
      <template v-slot:text>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatibus ipsum qui reprehenderit omnis laboriosam, quis amet dolor doloribus iure dolores odio cupiditate sint deserunt. Excepturi eum ratione nobis placeat labore?</template>
      <template v-slot:button>
        <NuxtLink class="btn btn--primary" to="/">Baza wiedzy</NuxtLink>
      </template>
    </Hero>
    <div class="home__img">
      <img loading="lazy" src="http://placekitten.com/600/600" alt="Kitty" width="600" height="600">
    </div>
  </Container>
</template>
<script lang="ts">
import Vue from 'vue'
import Container from '~/components/layout/Container.vue'
import Hero from '~/components/utils/Hero.vue'
export default Vue.extend({
    components: {
        Container,
        Hero
    }
})
</script>
<style lang="scss" scoped>
  .grid {
    display: grid;
    grid-template-columns: 60% auto;
    grid-template-rows: auto;
    margin-top: 2rem;
  }
  .hero {
    align-self: center;
  }
  .home {

  }
</style>