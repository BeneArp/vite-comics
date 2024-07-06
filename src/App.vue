<script>
import AppHeader from './components/AppHeader.vue'
import AppMainContent from './components/AppMainContent.vue'
import AppFooter from './components/AppFooter.vue'

export default{
    name: 'App',
    components: {
      AppHeader,
      AppMainContent,
      AppFooter,
    }
}

</script>

<template>
  <AppHeader/>
  <main>
      <AppMainContent/>
  </main>
  <AppFooter/>
</template>

<style lang="scss">

  @use './styles/general.scss' as *;
  @use './styles/partials/variables' as *;

  body{
    font-family: sans-serif;
  }

</style>
