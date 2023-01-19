<script >
import CompHeader from './components/CompHeader.vue';
import CompMain from './components/CompMain.vue';
import CompFooter from './components/CompFooter.vue';

export default {

  components: {
    CompHeader,
    CompMain,
    CompFooter
  }
}
</script>

<template>

  <CompHeader />
  <CompMain />
  <CompFooter />


</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables.scss' as *;
@use '../node_modules/bootstrap/scss/bootstrap.scss' as *;
</style>
