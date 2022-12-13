<script>
import AppHeader from './components/AppHeader.vue';
import Jumbo from './components/Jumbo.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: "App",
  components: {
    AppHeader,
    Jumbo,
    AppFooter,
  }
}

</script>

<template>
  <AppHeader />
  <Jumbo />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

main {
  // debug
  height: 100px;
  background-color: #1c1c1c;
  text-align: center;
  line-height: 100px;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primaryColor;
}
</style>
