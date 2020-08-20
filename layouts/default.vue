<template>
  <div class="layout">
    <h1 class="title"><nuxt-link to="/">I Cannot Design.</nuxt-link></h1>
    <github-link />
    <nuxt />
  </div>
</template>

<script>
import GithubLink from '~/components/GithubLink.vue';
export default {
  name: 'DefaultLayout',
  components: {GithubLink},
}
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
