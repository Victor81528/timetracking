<template>
  <Nav/>
</template>

<script>
import '@/_reset.css'
import Nav from './components/Nav.vue'

export default {
  name: 'App',
  components: {
    Nav
  }
}
</script>

<style lang="scss">
@font-face {
  font-family: SFProDisplay-Bold;
  src: url('./assets/fonts/SFProDisplay-Bold.ttf');
}
@font-face {
  font-family: SFProDisplay-Medium;
  src: url('./assets/fonts/SFProDisplay-Medium.ttf');
}
@font-face {
  font-family: SFProDisplay-Regular;
  src: url('./assets/fonts/SFProDisplay-Regular.ttf');
}
body {
  background-color: #E5E5E5;
}
#app {
}
</style>
