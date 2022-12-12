<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  }
}

</script>

<template>
  <AppHeader />
  <main>
    <h1>--> Content goes hear &lt;--</h1>
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

main {
  height: 100px;
  background-color: #1c1c1c;
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
