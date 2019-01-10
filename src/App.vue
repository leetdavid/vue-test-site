<template lang="pug">
  #app
    Nav
    main#page-wrap
      router-view
</template>

<script>
import Nav from './components/Nav'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
  name: 'App',
  components: {
    'Nav': Nav
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,400i,700,900');
@import url('/assets/css/style.css');
#app {
  font-family: Montserrat, sans-serif;
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: center;
}
body {
  margin: 0px;
}
h1 {
  font-weight: 400;
}
</style>
