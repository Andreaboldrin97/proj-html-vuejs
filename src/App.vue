<template>
  <div id="app">
    <headerContent/>
    <mainContent/>
    <footerContent/>
  </div>
</template>

<script>
import headerContent from './components/header.vue'
import mainContent from './components/main.vue'
import footerContent from './components/footer.vue'

export default {
  name: 'App',
  components: {
    headerContent,
    mainContent,
    footerContent
  }
}
</script>

<style lang="scss">

</style>
