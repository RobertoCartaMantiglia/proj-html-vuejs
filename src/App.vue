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

  <body>
    <CompHeader />
    <CompMain />
    <CompFooter />
  </body>


</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables.scss' as *;
@use '../node_modules/bootstrap/scss/bootstrap.scss' as *;
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,600;0,700;1,100;1,200;1,300;1,500&display=swap');
</style>
