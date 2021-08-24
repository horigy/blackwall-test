<template>
  <div id="app">
    <Header/>
    <Hero/>
    <Collab/>
    <Specials/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Collab from './components/Collab.vue'
import Specials from './components/Specials.vue'
export default {
  components: {
    Header,
    Hero,
    Collab,
    Specials
  }
}
</script>

<style lang="scss">
a {
  color: #18216D;
}
</style>
