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
@import url('https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;700&display=swap');

#app {
  font-family: 'Asap Condensed', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100vh;
}
</style>
