<template>
  <div id="app">
    <TheHeader />
    <TheMain />
    <TheBanner />
    <TheFooter />
    <SignUp />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheBanner from './components/TheBanner.vue'
import TheFooter from './components/TheFooter.vue'
import SignUp from './components/SignUp.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheBanner,
    TheFooter,
    SignUp
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
