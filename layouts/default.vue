<template>
  <div>
    <Header />
    <Nuxt />
  </div>
</template>
<script lang="ts">
import Vue from 'vue'
import Header from '~/components/layout/Header.vue'
export default Vue.extend({
  components: {
    Header
  }
})
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans:wght@400;700&display=swap');

html, body {
  font-family: 'Noto Sans', sans-serif;
  font-size: 14px;
  line-height: 1.4;
}

a {
  color: inherit;
  text-decoration: none;
  &:hover {
    text-decoration: underline;
  }
}

img {
  max-width: 100%;
  height: auto;
}

.btn {
  display: inline-block;
  padding: 1rem 2rem;
  color: white;
  background: black;
  text-transform: uppercase;
  &--lg {
    font-size: 1.2rem;
  }
}

</style>